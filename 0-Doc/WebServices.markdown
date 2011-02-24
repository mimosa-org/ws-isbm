#ISBM Web Services
--------------
##ISBMChannelManagementServiceSoap
###AssignSecurityToken  
####Request 
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:isbm="http://www.openoandm.org/xml/ISBM/">
       <soapenv:Header/>
       <soapenv:Body>
          <isbm:AssignSecurityTokens>
             <!--Optional:-->
             <isbm:channelID>?</isbm:channelID>
          </isbm:AssignSecurityTokens>
       </soapenv:Body>
    </soapenv:Envelope>
####Response
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
          <isbm:AssignSecurityTokensResponse xsi:nil="true" xmlns:isbm="http://www.openoandm.org/xml/ISBM/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
       </soapenv:Body>
    </soapenv:Envelope>

###CreateChannel
####Request
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:isbm="http://www.openoandm.org/xml/ISBM/">
       <soapenv:Header/>
       <soapenv:Body>
          <isbm:CreateChannel>
             <isbm:channelName>?</isbm:channelName>
             <isbm:channelType>?</isbm:channelType>
          </isbm:CreateChannel>
       </soapenv:Body>
    </soapenv:Envelope>
####Response
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
          <isbm:CreateChannelResponse xmlns:isbm="http://www.openoandm.org/xml/ISBM/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
             <isbm:channelID>ch20110224100916949</isbm:channelID>
             <isbm:TransactionStatus xsi:type="isbm:TransactionStatus_._1_._1_._1_._type">
                <isbm:successOrErrorCriteria>0</isbm:successOrErrorCriteria>
                <isbm:statusMessage>Channel created and bound!</isbm:statusMessage>
             </isbm:TransactionStatus>
          </isbm:CreateChannelResponse>
       </soapenv:Body>
    </soapenv:Envelope>

###CreateTopic
####Request
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:isbm="http://www.openoandm.org/xml/ISBM/">
       <soapenv:Header/>
       <soapenv:Body>
          <isbm:CreateTopic>
             <isbm:channelID>?</isbm:channelID>
             <isbm:topic>?</isbm:topic>
             <!--Optional:-->
             <isbm:description>?</isbm:description>
             <!--Optional:-->
             <isbm:xpathDefinition>?</isbm:xpathDefinition>
          </isbm:CreateTopic>
       </soapenv:Body>
    </soapenv:Envelope>
####Response
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
          <isbm:CreateTopicResponse xmlns:isbm="http://www.openoandm.org/xml/ISBM/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
             <isbm:TransactionStatus xsi:type="isbm:TransactionStatus_._1_._1_._1_._type">
                <isbm:successOrErrorCriteria>0</isbm:successOrErrorCriteria>
                <isbm:statusMessage>Success</isbm:statusMessage>
             </isbm:TransactionStatus>
          </isbm:CreateTopicResponse>
       </soapenv:Body>
    </soapenv:Envelope>

###CreateTopicNamespace
####Request
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:isbm="http://www.openoandm.org/xml/ISBM/">
       <soapenv:Header/>
       <soapenv:Body>
          <isbm:CreateTopicNamespace>
             <isbm:prefix>?</isbm:prefix>
             <isbm:namespace>?</isbm:namespace>
          </isbm:CreateTopicNamespace>
       </soapenv:Body>
    </soapenv:Envelope>
####Response
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
          <isbm:CreateTopicNamespaceResponse xsi:nil="true" xmlns:isbm="http://www.openoandm.org/xml/ISBM/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
       </soapenv:Body>
    </soapenv:Envelope>

###DeleteChannel
####Request
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:isbm="http://www.openoandm.org/xml/ISBM/">
       <soapenv:Header/>
       <soapenv:Body>
          <isbm:DeleteChannel>
             <isbm:channelID>?</isbm:channelID>
          </isbm:DeleteChannel>
       </soapenv:Body>
    </soapenv:Envelope>
####Response
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
          <isbm:DeleteChannelResponse xmlns:isbm="http://www.openoandm.org/xml/ISBM/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
             <isbm:TransactionStatus xsi:type="isbm:TransactionStatus_._1_._1_._1_._type">
                <isbm:successOrErrorCriteria>0</isbm:successOrErrorCriteria>
                <isbm:statusMessage>Success</isbm:statusMessage>
             </isbm:TransactionStatus>
          </isbm:DeleteChannelResponse>
       </soapenv:Body>
    </soapenv:Envelope>

###DeleteTopic
####Request
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:isbm="http://www.openoandm.org/xml/ISBM/">
       <soapenv:Header/>
       <soapenv:Body>
          <isbm:DeleteTopic>
             <isbm:channelID>?</isbm:channelID>
             <isbm:topic>?</isbm:topic>
          </isbm:DeleteTopic>
       </soapenv:Body>
    </soapenv:Envelope>
####Response
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
          <isbm:DeleteTopicResponse xmlns:isbm="http://www.openoandm.org/xml/ISBM/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
             <isbm:TransactionStatus xsi:type="isbm:TransactionStatus_._1_._1_._1_._type">
                <isbm:successOrErrorCriteria>0</isbm:successOrErrorCriteria>
                <isbm:statusMessage>Success</isbm:statusMessage>
             </isbm:TransactionStatus>
          </isbm:DeleteTopicResponse>
       </soapenv:Body>
    </soapenv:Envelope>

###GetAllChannels
####Request
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
          <isbm:DeleteTopicResponse xmlns:isbm="http://www.openoandm.org/xml/ISBM/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
             <isbm:TransactionStatus xsi:type="isbm:TransactionStatus_._1_._1_._1_._type">
                <isbm:successOrErrorCriteria>0</isbm:successOrErrorCriteria>
                <isbm:statusMessage>Success</isbm:statusMessage>
             </isbm:TransactionStatus>
          </isbm:DeleteTopicResponse>
       </soapenv:Body>
    </soapenv:Envelope>
####Response
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
          <isbm:GetAllChannelsResponse xmlns:isbm="http://www.openoandm.org/xml/ISBM/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
             <isbm:channelID>ch1</isbm:channelID>
             <isbm:channelID>ch2</isbm:channelID>
             <isbm:channelID>ch3</isbm:channelID>
             <isbm:channelID>ch4</isbm:channelID>
             <isbm:channelID>ch5</isbm:channelID>
             <isbm:TransactionStatus xsi:type="isbm:TransactionStatus_._1_._1_._1_._type">
                <isbm:successOrErrorCriteria>0</isbm:successOrErrorCriteria>
                <isbm:statusMessage>Success</isbm:statusMessage>
             </isbm:TransactionStatus>
          </isbm:GetAllChannelsResponse>
       </soapenv:Body>
    </soapenv:Envelope>

###GetAllSessions
####Request
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:isbm="http://www.openoandm.org/xml/ISBM/">
       <soapenv:Header/>
       <soapenv:Body>
          <isbm:GetAllSessions>
             <isbm:channelID>?</isbm:channelID>
          </isbm:GetAllSessions>
       </soapenv:Body>
    </soapenv:Envelope>
####Response
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
          <isbm:GetAllSessionsResponse xmlns:isbm="http://www.openoandm.org/xml/ISBM/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
             <isbm:channelSessionID>sub1</isbm:channelSessionID>
             <isbm:channelSessionID>sub2</isbm:channelSessionID>
             <isbm:channelSessionID>sub3</isbm:channelSessionID>
             <isbm:channelSessionID>sub4</isbm:channelSessionID>
             <isbm:channelSessionID>sub5</isbm:channelSessionID>
             <isbm:TransactionStatus xsi:type="isbm:TransactionStatus_._1_._1_._1_._type">
                <isbm:successOrErrorCriteria>0</isbm:successOrErrorCriteria>
                <isbm:statusMessage>Success</isbm:statusMessage>
             </isbm:TransactionStatus>
          </isbm:GetAllSessionsResponse>
       </soapenv:Body>
    </soapenv:Envelope>

###GetAllTopics
####Request
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:isbm="http://www.openoandm.org/xml/ISBM/">
       <soapenv:Header/>
       <soapenv:Body>
          <isbm:GetAllTopics>
             <isbm:channelID>?</isbm:channelID>
          </isbm:GetAllTopics>
       </soapenv:Body>
    </soapenv:Envelope>
####Response
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
          <isbm:GetAllTopicsResponse xmlns:isbm="http://www.openoandm.org/xml/ISBM/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
             <isbm:topic>Topic 1</isbm:topic>
             <isbm:topic>Topic 2</isbm:topic>
             <isbm:topic>Topic 3</isbm:topic>
             <isbm:topic>Topic 4</isbm:topic>
             <isbm:topic>Topic 5</isbm:topic>
             <isbm:TransactionStatus xsi:type="isbm:TransactionStatus_._1_._1_._1_._type">
                <isbm:successOrErrorCriteria>0</isbm:successOrErrorCriteria>
                <isbm:statusMessage>Success</isbm:statusMessage>
             </isbm:TransactionStatus>
          </isbm:GetAllTopicsResponse>
       </soapenv:Body>
    </soapenv:Envelope>

###GetChannelInfo
####Request
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:isbm="http://www.openoandm.org/xml/ISBM/">
       <soapenv:Header/>
       <soapenv:Body>
          <isbm:GetChannelInfo>
             <isbm:channelID>?</isbm:channelID>
          </isbm:GetChannelInfo>
       </soapenv:Body>
    </soapenv:Envelope>
####Response
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
          <isbm:GetChannelInfoResponse xmlns:isbm="http://www.openoandm.org/xml/ISBM/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
             <isbm:channelName>Some Channel</isbm:channelName>
             <isbm:channelType>1</isbm:channelType>
             <isbm:topic>Topic1</isbm:topic>
             <isbm:topic>Topic2</isbm:topic>
             <isbm:topic>Topic3</isbm:topic>
             <isbm:topic>Topic4</isbm:topic>
             <isbm:topic>Topic5</isbm:topic>
             <isbm:TransactionStatus xsi:type="isbm:TransactionStatus_._1_._1_._1_._type">
                <isbm:successOrErrorCriteria>0</isbm:successOrErrorCriteria>
                <isbm:statusMessage>Success</isbm:statusMessage>
             </isbm:TransactionStatus>
          </isbm:GetChannelInfoResponse>
       </soapenv:Body>
    </soapenv:Envelope>

###GetSessionsInfo
####Request
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:isbm="http://www.openoandm.org/xml/ISBM/">
       <soapenv:Header/>
       <soapenv:Body>
          <isbm:GetSessionInfo>
             <isbm:channelSessionID>?</isbm:channelSessionID>
          </isbm:GetSessionInfo>
       </soapenv:Body>
    </soapenv:Envelope>
####Response
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
          <isbm:GetSessionInfoResponse xmlns:isbm="http://www.openoandm.org/xml/ISBM/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
             <isbm:channelSessionType>Consumer</isbm:channelSessionType>
             <isbm:topic>dac8a760-2263-012e-8fb5-549a20e02a6a</isbm:topic>
             <isbm:listenerURI>Example.Session</isbm:listenerURI>
             <isbm:TransactionStatus xsi:type="isbm:TransactionStatus_._1_._1_._1_._type">
                <isbm:successOrErrorCriteria>0</isbm:successOrErrorCriteria>
                <isbm:statusMessage>Success</isbm:statusMessage>
             </isbm:TransactionStatus>
          </isbm:GetSessionInfoResponse>
       </soapenv:Body>
    </soapenv:Envelope>

###GetTopicInfo
####Request
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:isbm="http://www.openoandm.org/xml/ISBM/">
       <soapenv:Header/>
       <soapenv:Body>
          <isbm:GetTopicInfo>
             <isbm:channelID>ch1</isbm:channelID>
             <isbm:topic>SomeTopic</isbm:topic>
          </isbm:GetTopicInfo>
       </soapenv:Body>
    </soapenv:Envelope>
####Reponse
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
          <isbm:GetTopicInfoResponse xmlns:isbm="http://www.openoandm.org/xml/ISBM/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
             <isbm:channelID>ch1</isbm:channelID>
             <isbm:topic>SomeTopic</isbm:topic>
             <isbm:description>A Topic Generated for demonstration purposes</isbm:description>
             <isbm:xpathDefinition/>
             <isbm:TransactionStatus xsi:type="isbm:TransactionStatus_._1_._1_._1_._type">
                <isbm:successOrErrorCriteria>0</isbm:successOrErrorCriteria>
                <isbm:statusMessage>Success</isbm:statusMessage>
             </isbm:TransactionStatus>
          </isbm:GetTopicInfoResponse>
       </soapenv:Body>
    </soapenv:Envelope>

###RemoveSecurityTokens
####Request
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:isbm="http://www.openoandm.org/xml/ISBM/">
       <soapenv:Header/>
       <soapenv:Body>
          <isbm:RemoveSecurityTokens>
             <isbm:channelID>ch1</isbm:channelID>
          </isbm:RemoveSecurityTokens>
       </soapenv:Body>
    </soapenv:Envelope>
####Response
    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
          <isbm:RemoveSecurityTokensResponse xsi:nil="true" xmlns:isbm="http://www.openoandm.org/xml/ISBM/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
       </soapenv:Body>
    </soapenv:Envelope>
