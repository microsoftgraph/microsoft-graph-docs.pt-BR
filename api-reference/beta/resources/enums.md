---
title: Valores de enumeração
description: Valores de enumeração do Microsoft Graph
ms.openlocfilehash: 2f8bd0065136077cda2228cbec1c2d34d546c7d1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542801"
---
### <a name="contactrelationship-values"></a>valores de contactRelationship

|Member|Valor|Descrição|
|:---|:---|:---|
|primário|,0|O pai do usuário.|
|relativo|1 | O relativo do usuário.|
|facilita|2 | O auxílio do usuário.|
|Doutor|3 | O médico do usuário.|
|responsável|4 | O guardião do usuário.|
|pensão|5 | O filho do usuário.|
|outro|6 | Uma relação não especificada com o usuário.|
|unknownFutureValue|7 | Valor de marcador para compatibilidade futura.|

### <a name="timezonestandard-values"></a>valores de timeZoneStandard

| Valor
|:-----------------
| Windows
| IANA


### <a name="freebusystatus-values"></a>valores de freeBusyStatus

| Member            |Valor
|:------------------|:-------
| macro              | ,0
| provisória         | 1 
| Atualmente              | 2 
| temporária               | 3 
| workingElsewhere  | 4 
| desconhecido           | -1


### <a name="physicaladdresstype-values"></a>valores de physicalAddressType

| Valor
|:-------------------------
| desconhecido 
| Casa
| Business 
| outro


### <a name="attendeetype-values"></a>valores de attendetype

| Valor
|:-------------------------
| obrigatório
| opcional
| recurso


### <a name="externalaudiencescope-values"></a>valores de externalAudienceScope

| Valor
|:-------------------------
| Nenhuma
| contactsOnly
| todos os


### <a name="automaticrepliesstatus-values"></a>valores de automaticRepliesStatus

| Valor
|:-------------------------
| deficiência
| alwaysEnabled
| agendado


### <a name="calendarcolor-values"></a>valores de calendarColor

| Member     | Valor
|:-----------|:----------
| Automático       | -1
| lightBlue  | ,0
| lightGreen | 1 
| lightOrange| 2 
| lightGray  | 3 
| lightYellow| 4 
| lightTeal  | 5 
| lightPink  | 6 
| lightBrown | 7 
| lightRed   | 8 
| maxColor   | 9 


### <a name="educationsynchronizationprofilestate-values"></a>valores de educationSynchronizationProfileState

| Member     | Valor
|:-----------|:----------
| deleta          | 2 
| deletionFailed    | 3 
| provisioningFailed | 5 
| provisionado        | 6 
| provisionamento       | 7 
| unknownFutureValue | 8 


### <a name="educationsynchronizationstatus-values"></a>valores de educationSynchronizationStatus

| Member     | Valor
|:-----------|:----------
| pausado          | ,0
| inProgress    | 1 
| sucesso | 2 
| erro        | 3 
| validationError | 4 
| em quarentena       | 5 
| unknownFutureValue | 6 

### <a name="educationexternalsource-values"></a>valores de educationExternalSource

| Valor
|:-------------------------
| activa
| Manual
| unknownFutureValue


### <a name="educationgender-values"></a>valores de educationGender

| Valor
|:-------------------------
| feminino
| canto
| outro
| unknownFutureValue


### <a name="eventtype-values"></a>valores de eventType

| Valor
|:-------------------------
| singleInstance
| ocorrência
| exceções
| série


### <a name="sensitivity-values"></a>valores de sensibilidade

| Valor
|:-------------------------
| SS
| pessoal
| privada
| acordo


### <a name="importance-values"></a>valores de importância

| Valor
|:-------------------------
| low
| SS
| high


### <a name="educationuserrole-values"></a>valores de educationUserRole
| Valor
|:---------------------
| student
| teacher
| Nenhuma
| unknownFutureValue


### <a name="meetingmessagetype-values"></a>valores de meetingMessageType

| Valor
|:-----------------
| Nenhuma
| meetingRequest
| meetingCancelled
| meetingAccepted
| meetingTentativelyAccepted
| meetingDeclined


### <a name="followupflagstatus-values"></a>valores de followupFlagStatus

| Valor
|:-------------------------
| não sinalizado
| complete
| indicado


### <a name="inferenceclassificationtype-values"></a>valores de inferenceClassificationType

| Valor
|:-----------------
| Destaques
| outro


### <a name="iosnotificationalerttype-values"></a>valores de iosNotificationAlertType

| Valor
|:-------------------------
| deviceDefault
| Bandeira
| JanelaRestrita
| Nenhuma

### <a name="deviceenrollmentfailurereason-values"></a>valores de deviceEnrollmentFailureReason

| Valor
|:-------------
| desconhecido
| autentica
| nesse
| accountValidation
| userValidation
| deviceNotSupported
| inManutenção
| badRequest
| featureNotSupported
| enrollmentRestrictionsEnforced
| clientDisconnected


### <a name="bodytype-values"></a>valores de BodyType
| Valor
|:---------
| texto
| HTML


### <a name="locationtype-values"></a>valores LocationType

| Valor
|:-------------------------
| Padrão.
| conferenceRoom
| homeAddress
| businessAddress
| geoCoordinates
| streetAddress
| diárias
| restaurantes
| localBusiness
| postalAddress

### <a name="locationuniqueidtype-values"></a>valores de locationUniqueIdType

| Valor
|:-------------------------
| desconhecido
| locationStore
| Directory
| privada
| Bing


### <a name="messageactionflag-values"></a>valores de messageActionFlag

| Valor
|:-------------------------
| qualquer
| call
| doNotForward
| Acompanhamento
| conhecimento
| forward
| noResponseNecessary
| Saiba
| reply
| replyToAll
| exame


### <a name="onenoteuserrole-values"></a>valores de onenoteUserRole

| Member      | Valor
|:------------|:------------
| Owner       | ,0
| Colaborador | 1 
| Leitor      | 2 
| Nenhum        | -1


### <a name="operationstatus-values"></a>valores de operationStatus

| Valor
|:-----------------
| NotStarted
| Executando
| Completed
| Failed


### <a name="onenotepatchactiontype-values"></a>valores de onenotePatchActionType

| Valor
|:-------------------------
| Substituir
| Append
| Excluir
| Inserir
| Preceder

### <a name="onenotepatchinsertposition-values"></a>valores de onenotePatchInsertPosition

| Valor
|:-------------------------
| After
| Before


### <a name="phonetype-values"></a>valores de PhoneType

| Valor
|:-------------------------
| Casa
| Business
| processadores
| outro
| assistência
| homeFax
| businessFax
| otherFax
| pager
| Radio


### <a name="plannerpreviewtype-values"></a>valores de plannerPreviewType

| Valor
|:-------------------------
| Automático
| noPreview
| verificação
| description
| de referência


### <a name="status-values"></a>valores de status

| Valor
|:-----------------
| active
| atualizado
| deleted
| ignor
| unknownFutureValue


### <a name="weekindex-values"></a>valores de weekIndex

| Valor
|:-------------------------
| primeiro
| secundária
| terceiriza
| etapa
| durar


### <a name="dayofweek-values"></a>valores de dayOfWeek

| Valor
|:-------------------------
| domingo
| período
| feira
| feira
| quinta-feira
| sexta
| sábado

### <a name="recurrencepatterntype-values"></a>valores recurrencePattern

| Valor
|:-------------------------
| diariamente
| mensal
| absoluteMonthly
| relativeMonthly
| absoluteYearly
| relativeYearly


### <a name="recurrencerangetype-values"></a>valores de recurrenceRangeType

| Valor
|:-------------------------
| endDate
| noEnd
| numerada


### <a name="onenotesourceservice-values"></a>valores de onenoteSourceService
| Valor
|:---------------------
| Desconhecido
| OneDrive
| OneDriveForBusiness
| OnPremOneDriveForBusiness


### <a name="responsetype-values"></a>valores ResponseType

| Valor
|:-------------------------
| Nenhuma
| organizer
| tentativelyAccepted
| aceito
| recusada
| Não respondido


### <a name="activitydomain-values"></a>valores de activityDomain

| Valor
|:-------------------------
| desconhecido
| trabalho
| pessoal
| irrestrito


### <a name="websitetype-values"></a>valores de WebSiteType

| Valor
|:-------------------------
| outro
| Casa
| trabalho
| blog
| perfil


### <a name="categorycolor-values"></a>valores de categoryColor

| Member   |Valor    
|:---------|:--------
| Nenhuma     | -1      
| preset0  | ,0       
| preset1  | 1        
| preset2  | 2        
| preset3  | 3        
| preset4  | 4        
| preset5  | 5        
| preset6  | 6        
| preset7  | 7        
| preset8  | 8        
| preset9  | 9        
| preset10 | 10       
| preset11 | 11       
| preset12 | 12       
| preset13 | 13       
| preset14 | 14       
| preset15 | 15       
| preset16 | 16       
| preset17 | 17       
| preset18 | 18       
| preset19 | 19      
| preset20 | 508      
| preset21 | 21      
| preset22 | 22      
| preset23 | 23      
| preset24 | dia      

### <a name="alertfeedback-values"></a>valores de alertFeedback

Possíveis valores de comentários no alerta fornecido por um analista.

|Member|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Unknown.|
|truePositive|1 |O alerta é verdadeiro e positivo.|
|falsePositive|2 | O alerta é falso positivo.|
|benignPositive|3 | O alerta é benigno-positivo.|

### <a name="filehashtype-values"></a>valores de fileHashtype

|Member|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Tipo desconhecido.|
|SHA1|1 |Tipo de hash SHA1.|
|SHA256|2 | Tipo de hash SHA256.|
|MD5|3 | Tipo de hash MD5.|
|authenticodeHash256|4 | Tipo de hash AuthenticodeHash256.|
|lsHash|5 | Tipo de hash LsHash.|
|ctph|6 | Tipo de hash CTPH.|
|peSha1|7 | Tipo de hash PESHA1.|
|peSha256|8 | Tipo de hash PESHA256.|

### <a name="connectiondirection-values"></a>valores de connectionDirection

|Member|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Conexão desconhecida.|
|entrada|1 |Conexão de entrada.|
|saída|2 | Conexão de saída.|

### <a name="connectionstatus-values"></a>valores de connectionStatus

|Member|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Status de conexão desconhecido.|
|tentou|1 |Tentativa de conexão.|
|adicionada|2 | Conexão bem-sucedida.|
|bloqueou|3 | Conexão bloqueada.|
|falhou|4 | Falha de conexão.|

### <a name="processintegritylevel-values"></a>valores de processIntegrityLevel

|Member|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Unknown.|
|não confiáveis|10 |O nível de integridade é não confiável.|
|low|508| O nível de integridade é baixo.|
|medium|até| O nível de integridade é médio.|
|high|40| O nível de integridade é alto.|
|sistema|50| O nível de integridade é System.|

### <a name="registryhive-values"></a>valores de registryHive

Enumeração para hives do registro, conforme [https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives)definido por.

|Member|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Hive desconhecido.|
|currentConfig|1 |Hive HKEY_CURRENT_CONFIG.|
|currentUser|2 | Hive HKEY_CURRENT_USER.|
|localMachineSam|3 | Hive HKEY_LOCAL_MACHINE\SAM.|
|localMachineSamSoftware|4 | Hive HKEY_LOCAL_MACHINE\Software.|
|localMachineSystem|5 | HKEY_LOCAL_MACHINE\System Hive.|
|usersDefault|6 | HKEY_USERS\\. Hive padrão.|

### <a name="registryoperation-values"></a>valores de registryOperation

Operação que alterou o nome da chave do registro e/ou o valor.

|Member|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Tipo de valor de registro desconhecido.|
|create|1 |Criar registro.|
|modifica|2 |Modificar o registro.|
|delete|3 |Excluir registro.|

### <a name="registryvaluetype-values"></a>valores de registryValueType

Enumeração para tipos de valor do registro conforme [https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types)definido por.

|Member|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Tipo de valor de registro desconhecido.|
|binário|1 |Tipo de valor de registro REG_BINARY.|
|últimas|2 | Tipo de valor do registro REG_DWORD.|
|dwordLittleEndian|3 | Tipo de valor do registro REG_DWORD_LITTLE_ENDIAN.|
|dwordBigEndian|4 | Tipo de valor do registro REG_DWORD_BIG_ENDIAN.|
|expandSz|5 | Tipo de valor do registro REG_EXPAND_SZ.|
|vínculo|6 | Tipo de valor do registro REG_LINK.|
|multiSz|7 | Tipo de valor de registro REG_MULTI_SZ.|
|Nenhuma|8 | Tipo de valor do registro REG_NONE.|
|QWORD|9 | Tipo de valor do registro REG_QWORD.|
|qwordlittleEndian|10 | Tipo de valor do registro REG_QWORD_LITTLE_ENDIAN.|
|v|11 | Tipo de valor do registro REG_SZ.|

### <a name="alertseverity-values"></a>valores de alertSeverity

Enumeração para gravidade de alertas.

|Member|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|A severidade é desconhecida.|
|informativa|1 |A severidade só é para informações.|
|low|2 | A severidade é baixa.|
|medium|3 | A severidade é média.|
|high|4 | A severidade é alta.|

### <a name="alertstatus-values"></a>valores de alertStatus

Valores possíveis de um status de ciclo de vida de alerta (estágio).

|Member|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Status desconhecido.|
|newAlert|10 | O alerta é novo.|
|inProgress|508|O alerta está em andamento.|
|Obtido|até|O alerta foi resolvido.|

### <a name="emailrole-values"></a>valores de emailRole

Valores possíveis para funções de email.

|Member|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Função desconhecida.|
|sender|1 |Remetente do email.|
|destinatário|2 |Destinatário do email.|

### <a name="logontype-values"></a>valores de Logontype

Valores possíveis para o método de User Sign.

|Member|Valor|Descrição|
|:---|:---|:---|
|desconhecido|-1|Unknown.|
|interativa|,0|O logon é interativo.|
|remoteInteractive|1 | O logon é interativo remoto.|
|rede|2 | O logon é rede.|
|batch|3 | O logon é em lote.|
|service|4 | O logon é serviço.|

### <a name="useraccountsecuritytype-values"></a>valores de userAccountSecurityType

Valores possíveis para tipos de contas de usuário (Associação de grupo), por definição do Windows.

|Member|Valor|Descrição|
|:---|:---|:---|
|desconhecido|-1|Unknown.|
|caracteres|,0|Membro do grupo de usuários padrão.|
|força|1 | Membro do grupo de usuários avançados.|
|administrador|2 | Membro do grupo Administradores.|
