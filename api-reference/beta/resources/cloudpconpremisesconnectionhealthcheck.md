---
title: Tipo de recurso cloudPcOnPremisesConnectionHealthCheck
description: O resultado de uma verificação de conexões de rede do Azure pc na nuvem.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: fc8ee01576e6381c54455d765a007e89b8f9c0d7
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589265"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>Tipo de recurso cloudPcOnPremisesConnectionHealthCheck

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O resultado de uma verificação de conexões de rede do Azure pc na nuvem.

[!INCLUDE [on-premise-rename-note](../../includes/on-premise-rename-note.md)]

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[RunHealthChecks de cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Nenhum|Execute as verificações de saúde de [um cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição desse item de verificação de saúde.|
|status|[cloudPcOnPremisesConnectionStatus](../resources/cloudpconpremisesconnection.md#cloudpconpremisesconnectionstatus-values)|O status do item de verificação de saúde. Os valores possíveis são: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`. Somente leitura.|
|startDateTime|DateTimeOffset|A hora de início do item de verificação de saúde. Somente leitura.|
|endDateTime|DateTimeOffset|A hora de término do item de verificação de saúde. Somente leitura.|
|errorType|[cloudPcOnPremisesConnectionHealthCheckErrorType](#cloudpconpremisesconnectionhealthcheckerrortype-values)|O tipo de erro que ocorreu durante essa verificação de saúde.|
|recommendedAction|Cadeia de caracteres|A ação recomendada para corrigir o erro correspondente.|
|additionalDetails|Cadeia de caracteres|Detalhes adicionais sobre a verificação de saúde ou a ação recomendada.|

### <a name="cloudpconpremisesconnectionhealthcheckerrortype-values"></a>valores cloudPcOnPremisesConnectionHealthCheckErrorType

|Member|Descrição|
|:---|:---|
|dnsCheckFqdnNotFound|A resolução DNS falhou para o nome de domínio. Possíveis causas de erro: 1. O servidor DNS do Azure vNet especificado não pode resolver o nome de domínio. Atualize a vNet com um servidor DNS apropriado; 2. O nome de domínio fornecido não existe ou não está correto. Atualize a conexão de rede do Azure com o nome de domínio correto. Verifique se a vNet definida na conexão de rede do Azure pode resolver o nome de domínio.|
|dnsCheckNameWithInvalidCharacter|A verificação DNS falhou porque o nome de domínio inserido contém um caractere sem suporte. Verifique se o nome de domínio contém apenas caracteres com suporte.|
|dnsCheckUnknownError|A resolução DNS falhou para o nome de domínio. Possíveis causas de erro: 1. O servidor DNS do Azure vNet especificado não pode resolver o nome de domínio. Atualize a vNet com um servidor DNS apropriado; 2. O nome de domínio fornecido não existe ou não está correto. Atualize a conexão de rede do Azure com o nome de domínio correto. Verifique se a vNet definida na conexão de rede do Azure pode resolver o nome de domínio.|
|adJoinCheckFqdnNotFound|A verificação de junção de domínio falhou porque o nome de domínio não pôde ser encontrado. Verifique se um controlador de domínio para o nome de domínio pode ser contatado pela vNet definida na conexão de rede do Azure.|
|adJoinCheckIncorrectCredentials|A verificação de junção de domínio falhou porque as credenciais fornecidas para o domínio não estão corretas. Atualize a conexão de rede do Azure com credenciais corretas.|
|adJoinCheckOrganizationalUnitNotFound|A verificação de junção de domínio falhou porque a unidade organizacional (OU) não pode ser encontrada. Forneça uma UO no domínio. A UO deve estar no formato de nome diferenciado. Formato de exemplo: "OU=OU1,OU=OU2,OU=OU3,DC=DC1".|
|adJoinCheckOrganizationalUnitIncorrectFormat|A verificação de junção de domínio falhou porque a unidade organizacional (OU) não pode ser encontrada. Forneça uma UO no domínio. A UO deve estar no formato de nome diferenciado. Formato de exemplo: "OU=OU1,OU=OU2,OU=OU3,DC=DC1".|
|adJoinCheckComputerObjectAlreadyExists|A conta do computador não pode ser encontrada na unidade organizacional (OU) fornecida na conexão de rede do Azure, mas o nome do computador já existe no domínio. Isso geralmente ocorre depois que o objeto do computador foi movido para fora da UO configurada na conexão de rede do Azure. Mova o objeto do computador de volta para a UO de destino.|
|adJoinCheckAccessDenied|A verificação de junção de domínio falhou porque a conta de usuário fornecida não tem permissões suficientes para ingressar no domínio. Verifique se a conta fornecida tem permissões suficientes ou altere a conta de usuário definida nas propriedades de conexão de rede do Azure. Permissões necessárias: Criar *objetos de computador e* *Excluir objetos do computador*.|
|adJoinCheckCredentialsExpired|A verificação de junção de domínio falhou porque a senha do usuário de junção de domínio expirou. Primeiro atualize a senha e atualize a conexão de rede do Azure com as novas credenciais.|
|adJoinCheckAccountLockedOrDisabled|A verificação de junção de domínio falhou porque a conta de usuário de junção de domínio está bloqueada ou desabilitada no momento. Verifique se a conta de usuário de junção de domínio está desbloqueada, ativa e capaz de se autenticar no domínio.|
|adJoinCheckAccountQuotaExceeded|A verificação de junção de domínio falhou porque o usuário de junção de domínio excedeu o máximo de junções de domínio. Verifique se a junção de domínio é permitida e a **propriedade ms-DS-MachineAccountQuota** Active Directory permite junções de domínio suficientes.|
|adJoinCheckUnknownError|A verificação de junção de domínio falhou devido a um erro desconhecido. Certifique-se de que a conexão de rede do Azure possa ingressar com êxito no domínio usando os detalhes fornecidos.|
|endpointConnectivityCheckCloudPcUrlNotAllowListed|Durante o provisionamento, uma ou mais URLs necessárias não puderam ser contatadas. Verifique se todas as URLs necessárias são permitidas por meio dos firewalls e proxies.|
|endpointConnectivityCheckWVDUrlNotAllowListed|Durante o provisionamento, uma ou mais URLs WVD necessárias não puderam ser contatadas. Verifique se todas as URLs necessárias são permitidas por meio dos firewalls e proxies.|
|endpointConnectivityCheckIntuneUrlNotAllowListed|Durante o provisionamento, uma ou mais URLs Intune não puderam ser contatadas. Verifique se todas as URLs necessárias são permitidas por meio dos firewalls e proxies.|
|endpointConnectivityCheckUnknownError|Durante o provisionamento, uma ou mais URLs necessárias não puderam ser contatadas. Verifique se todas as URLs necessárias são permitidas por meio dos firewalls e proxies.|
|azureAdDeviceSyncCheckDeviceNotFound|O objeto do computador do computador na nuvem não pode ser encontrado no Azure Active Directory (Azure AD). Certifique-se de que a conexão do Azure AD funcione e sincronize com frequência para que os objetos do computador do computador na nuvem sejam sincronizados com o Azure AD. A sincronização de dispositivos do Azure AD deve ser habilitada e sincronizada nos últimos 60 minutos.|
|azureAdDeviceSyncCheckLongSyncCircle|A verificação se o objeto do computador do computador na nuvem foi sincronizado com Azure Active Directory (Azure AD) foi o tempo de tempo. Certifique-se de que a conexão do Azure AD funcione e sincronize com frequência para que os objetos do computador do computador na nuvem sejam sincronizados com o Azure AD. A sincronização de dispositivos do Azure AD deve ser habilitada e sincronizada nos últimos 60 minutos.|
|azureAdDeviceSyncCheckConnectDisabled|A Azure Active Directory de sincronização de dispositivos (Azure AD) falhou porque o Conexão do Azure AD está desabilitado. Verifique se a Conexão do Azure AD está habilitada e sincroniza com frequência. Se o Azure AD Conexão não sincronizar o computador em 60 minutos, a verificação falhará.|
|azureAdDeviceSyncCheckDurationExceeded|A Azure Active Directory de sincronização do dispositivo (Azure AD) falhou porque a sincronização de Conexão do Azure AD não foi sincronizada dentro de 60 minutos. Verifique se a Conexão do Azure AD está habilitada e sincroniza com frequência. Se o Azure AD Conexão não sincronizar o computador em 60 minutos, a verificação falhará.|
|azureAdDeviceSyncCheckScpNotConfigured|A junção Azure Active Directory Híbrida (Azure AD) falhou devido a erros de configuração no Ponto de Configuração do Serviço (SCP). Verifique se sua configuração SCP é válida e disponível para executar uma junção híbrida do Azure AD. Seu SCP pode ser criado e configurado no assistente de Conexão do Azure AD.|
|azureAdDeviceSyncCheckTransientServiceError|A Azure Active Directory de sincronização do dispositivo (Azure AD) falhou devido a um erro transitório. Tente novamente. Se o problema persistir, entre em contato com o suporte do cliente.|
|azureAdDeviceSyncCheckUnknownError|Falha na Azure Active Directory de conectividade híbrida (Azure AD). Certifique-se de que a conexão do Azure AD funcione e sincronize com frequência para que os objetos do computador do computador na nuvem sejam sincronizados com o Azure AD. A sincronização de dispositivos do Azure AD deve ser habilitada e sincronizada nos últimos 60 minutos.|
|resourceAvailabilityCheckNoSubnetIP|A sub-rede fornecida não tem endereços IP disponíveis. Verifique se a sub-rede fornecida na conexão de rede do Azure tem endereços IP suficientes disponíveis. Expanda a sub-rede selecionada atual ou selecione uma sub-rede diferente a ser usada para provisionamento.|
|resourceAvailabilityCheckSubscriptionDisabled|A assinatura do Azure fornecida está desabilitada. Verifique se a assinatura do Azure está habilitada e disponível para provisionamento.|
|resourceAvailabilityCheckAzurePolicyViolation|A assinatura do Azure fornecida não pode ser encontrada. Verifique se a assinatura do Azure está disponível para provisionamento.|
|resourceAvailabilityCheckSubscriptionNotFound|A assinatura do Azure fornecida não pode ser acessada. Verifique se a assinatura do Azure está disponível para provisionamento.|
|resourceAvailabilityCheckSubscriptionTransferred|A assinatura do Azure fornecida não pode ser acessada. Verifique se a assinatura do Azure está disponível para provisionamento.|
|resourceAvailabilityCheckGeneralSubscriptionError|Uma política do Azure está restringindo a criação de recursos. Verifique se não há nenhuma política do Azure que restrinja a criação de recursos no grupo de assinaturas e/ou recursos.|
|resourceAvailabilityCheckUnsupportedVNetRegion|O vNet selecionado está localizado em uma região sem suporte. Verifique se o vNet selecionado está localizado em uma região com suporte.|
|resourceAvailabilityCheckResourceGroupInvalid|O grupo de recursos selecionado do Azure é inválido ou não encontrado. Verifique se o grupo de recursos selecionado do Azure está disponível para provisionar recursos. Como alternativa, atualize essa conexão de rede do Azure com outro grupo de recursos.|
|resourceAvailabilityCheckVNetInvalid|A rede virtual do Azure selecionada é inválida. Verifique se a rede virtual selecionada está disponível e saudável. Como alternativa, atualize essa conexão de rede do Azure com outra rede virtual.|
|resourceAvailabilityCheckSubnetInvalid|A sub-rede selecionada do Azure é inválida. Verifique se a sub-rede selecionada está disponível e saudável. Como alternativa, atualize essa conexão de rede do Azure com outra sub-rede.|
|resourceAvailabilityCheckResourceGroupBeingDeleted|O grupo de recursos selecionado do Azure está sendo excluído. Verifique se o grupo de recursos selecionado do Azure está disponível para provisionar recursos. Como alternativa, atualize essa conexão de rede do Azure com outro grupo de recursos.|
|resourceAvailabilityCheckVNetBeingMoved|A rede virtual do Azure selecionada está sendo movida. Verifique se sua rede virtual não está mudando ou sendo movida e tente novamente. Como alternativa, atualize essa conexão de rede do Azure com outro vNet.|
|resourceAvailabilityCheckSubnetDelegationFailed|A rede virtual do Azure selecionada tem delegação de sub-rede que bloqueia a criação de uma interface de rede (Nic). Peça ao proprietário da rede virtual do Azure para modificar sua política de delegação de sub-rede para permitir que o provisionamento seja bem-sucedido.|
|resourceAvailabilityCheckSubnetWithExternalResources|A sub-rede selecionada não pode ser usada porque contém recursos externos. Remova todos os recursos que podem causar conflitos e tente novamente. Como alternativa, atualize essa conexão de rede do Azure com outra sub-rede.|
|resourceAvailabilityCheckResourceGroupLockedForReadonly|O grupo de recursos selecionado está bloqueado e não pode ser modificado para provisionamento. Remova esse bloqueio para permitir que o provisionamento seja bem-sucedido.|
|resourceAvailabilityCheckResourceGroupLockedForDelete|O grupo de recursos selecionado ou seu escopo pai foi bloqueado para ações de exclusão. Pode ser porque os endereços IP são usados. Remova o bloqueio e tente novamente.|
|resourceAvailabilityCheckTransientServiceError|A verificação de disponibilidade do recurso falhou devido a um erro transitório. Tente novamente. Se o problema persistir, entre em contato com o suporte do cliente.|
|resourceAvailabilityCheckUnknownError|A verificação de disponibilidade de recursos do Azure falhou devido a um erro desconhecido. Verifique se todos os recursos do Azure atendem aos pré-requisitos.|
|permissionCheckNoSubscriptionReaderRole|A entidade de serviço de computador na nuvem não tem permissões suficientes na assinatura do Azure. Certifique-se de que a entidade de serviço do computador na nuvem tenha as *permissões Reader* na assinatura.|
|permissionCheckNoResourceGroupOwnerRole|A entidade de serviço de computador na nuvem não tem permissões suficientes no grupo de recursos do Azure. Verifique se a entidade de serviço do computador na nuvem tem as *permissões Owner* no grupo de recursos. |
|permissionCheckNoVNetContributorRole|A entidade de serviço de computador na nuvem não tem permissões suficientes na vNet do Azure. Verifique se o serviço de computador na nuvem tem as *permissões do* colaborador de rede na vNet.|
|permissionCheckNoResourceGroupNetworkContributorRole|A entidade de serviço de computador na nuvem não tem permissões suficientes no grupo de recursos do Azure. Verifique se o aplicativo tem permissões de colaboradores de rede no grupo de recursos.|
|permissionCheckTransientServiceError|A verificação de permissão do aplicativo de primeira parte falhou devido a um erro transitório. Tente novamente. Se o problema persistir, entre em contato com o suporte do cliente.|
|permissionCheckUnknownError|A entidade de serviço de computador na nuvem não tem permissões suficientes. Verifique se a entidade de serviço do computador na nuvem recebe permissões suficientes do Azure.|
|internalServerErrorDeploymentCanceled|A implantação foi cancelada. Tente novamente mais tarde. Se o problema persistir, entre em contato com o suporte.|
|internalServerErrorAllocateResourceFailed|A alocação de recursos falhou. Tente novamente mais tarde. Se o problema persistir, entre em contato com o suporte.|
|internalServerErrorVMDeploymentTimeout|O tempo de implantação da máquina virtual foi o tempo de implantação. Tente novamente mais tarde. Se o problema persistir, entre em contato com o suporte.|
|internalServerErrorUnableToRunDscScript|Durante o provisionamento, alguns scripts DSC do PowerShell são executados no computador de nuvem. Não é possível baixar esses scripts DSC ou executá-los durante a verificação de saúde. Verifique se a vNet tem acesso irrestrito aos pontos de extremidade necessários, e o PowerShell não está bloqueado no ambiente ou Política de Grupo.|
|internalServerUnknownError|O provisionamento falhou devido a um erro interno. Entre em contato com o suporte ao cliente.|
|unknownFutureValue|Valor de sentinela de enumeração evolvável. Não usar.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
  "displayName": "String",
  "status": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "errorType": "String",
  "recommendedAction": "String",
  "additionalDetails": "String"
}
```
