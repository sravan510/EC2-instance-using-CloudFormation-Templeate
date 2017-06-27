Topic : Create a cloudfromation template that builds an entire VPC, including subnets, internet gateway and routing tables. After buliding VPC the template should launch EC2 instance into the public VPC.


Steps Followed:

Step1 : (AWS::EC2::VPC) Create a VPC.

Step2 : (AWS::EC2::Subnet) Create a Subnet.

Step3 : (AWS::EC2::InternetGateway) Create a InternetGateway.

Step4 : (AWS::EC2::VPCGatewayAttachment) Attach VPC to the InternetGateway.

Step5 : (AWS::EC2::RouteTable) Create a RouteTable to the VPC.

Step6 : (AWS::EC2::Route) Create a new route to the routetable within a VPC, to the created internet gateway.  

Step7 : (AWS::EC2::SubnetRouteTableAssociation) Associates a subnet with a route table.

Step8 : (AWS::EC2::Instance) Launch EC2 instance in the created VPC.
			
			
Note : Code uploaded to the github is not in JSON format.
