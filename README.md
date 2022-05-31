# Container-Docker-Passbolt

# INSTRUCTIONS

select token from authentication_tokens where user_id = (select id from users where username = 'your@email.com') and type = 'recover' order by created DESC;



docker-compose exec passbolt su -m -c "/usr/share/php/passbolt/bin/cake \
                                passbolt register_user \
                                -u systems@trusc.net \
                                -f trusc \
                                -l godmode \
                                -r admin" -s /bin/sh www-data





docker-compose exec passbolt su -m -c "/usr/share/php/passbolt/bin/cake passbolt send_test_email --recipient=dean.nielsen@trusc.net"

