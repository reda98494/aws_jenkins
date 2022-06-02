resource "aws_instance" "JENKINS-<##INSTANCE_NUMBER##>-adm" {
        key_name = "test_keypair"
        ami = "ami-021d41cbdefc0c994"
        security_groups = ["sg-092271493b7c6d49a"]
        subnet_id = "subnet-0c59a465aaea21d4a"
        instance_type = "t2.micro"
        associate_public_ip_address = "true"
        user_data = "${file("<##USER_DATA##>")}"
        tags = {
                Name = "JENKINS-<##INSTANCE_NUMBER##>-adm"
        }
}
