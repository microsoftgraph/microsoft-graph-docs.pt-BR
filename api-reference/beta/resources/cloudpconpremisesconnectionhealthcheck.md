---
title: Tipo de recurso cloudPcOnPremisesConnectionHealthCheck
description: O resultado de uma verificação de saúde de conexão local do computador na nuvem.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: d091f174fa308c44418e5332657f45bbf82cdaf9
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767052"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>Tipo de recurso cloudPcOnPremisesConnectionHealthCheck

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O resultado de uma verificação de saúde de conexão local do computador na nuvem.

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
|dnsCheckFqdnNotFound|A resolução DNS falhou para o nome de domínio. Possíveis causas de erro: 1. O servidor DNS do Azure vNet especificado não pode resolver o nome de domínio. Atualize a vNet com um servidor DNS apropriado; 2. O nome de domínio fornecido não existe ou não está correto. Atualize a conexão de rede local com o nome de domínio correto. Verifique se a vNet definida na conexão de rede local pode resolver o nome de domínio.|
|dnsCheckUnknownError|A resolução DNS falhou para o nome de domínio. Possíveis causas de erro: 1. O servidor DNS do Azure vNet especificado não pode resolver o nome de domínio. Atualize a vNet com um servidor DNS apropriado; 2. O nome de domínio fornecido não existe ou não está correto. Atualize a conexão de rede local com o nome de domínio correto. Verifique se a vNet definida na conexão de rede local pode resolver o nome de domínio.|
|adJoinCheckFqdnNotFound|A verificação de junção de domínio falhou porque o nome de domínio não pôde ser encontrado. Verifique se um controlador de domínio para o nome de domínio pode ser contatado pela vNet definida na conexão de rede local.|
|adJoinCheckIncorrectCredentials|A verificação de junção de domínio falhou porque as credenciais fornecidas para o domínio não estão corretas. Atualize a conexão de rede local com credenciais corretas.|
|adJoinCheckOrganizationalUnitNotFound|A verificação de junção de domínio falhou porque a unidade organizacional (OU) não pode ser encontrada. Forneça uma UO no domínio. A UO deve estar no formato de nome diferenciado. Formato de exemplo: "OU=OU1,OU=OU2,OU=OU3,DC=DC1".|
|adJoinCheckOrganizationalUnitIncorrectFormat|A verificação de junção de domínio falhou porque a unidade organizacional (OU) não pode ser encontrada. Forneça uma UO no domínio. A UO deve estar no formato de nome diferenciado. Formato de exemplo: "OU=OU1,OU=OU2,OU=OU3,DC=DC1".|
|adJoinCheckComputerObjectAlreadyExists|A conta do computador não pode ser encontrada na unidade organizacional (OU) fornecida na conexão de rede local, mas o nome do computador já existe no domínio. Isso geralmente ocorre depois que o objeto do computador foi movido para fora da UO configurada na conexão de rede local. Mova o objeto do computador de volta para a UO de destino.|
|adJoinCheckAccessDenied|A verificação de junção de domínio falhou porque a conta de usuário fornecida não tem permissões suficientes para ingressar no domínio. Verifique se a conta fornecida tem permissões suficientes ou altere a conta de usuário definida nas propriedades de conexão de rede local. Permissões necessárias: Criar *objetos de computador e* Excluir objetos de *computador*.|
|adJoinCheckUnknownError|A verificação de junção de domínio falhou devido a um erro desconhecido. Certifique-se de que a conexão de rede local possa ingressar com êxito no domínio usando os detalhes fornecidos.|
|endpointConnectivityCheckCloudPcUrlNotAllowListed|Durante o provisionamento, uma ou mais URLs necessárias não puderam ser contatadas. Verifique se todas as URLs necessárias são permitidas por meio dos firewalls e proxies.|
|endpointConnectivityCheckWVDUrlNotAllowListed|Durante o provisionamento, uma ou mais URLs WVD necessárias não puderam ser contatadas. Verifique se todas as URLs necessárias são permitidas por meio dos firewalls e proxies.|
|endpointConnectivityCheckIntuneUrlNotAllowListed|Durante o provisionamento, uma ou mais URLs necessárias do Intune não puderam ser contatadas. Verifique se todas as URLs necessárias são permitidas por meio dos firewalls e proxies.|
|endpointConnectivityCheckUnknownError|Durante o provisionamento, uma ou mais URLs necessárias não puderam ser contatadas. Verifique se todas as URLs necessárias são permitidas por meio dos firewalls e proxies.|
|azureAdDeviceSyncCheckDeviceNotFound|O objeto do computador do computador na nuvem não pode ser encontrado no Azure Active Directory (Azure AD). Certifique-se de que a conexão do Azure AD funcione e sincronize com frequência para que os objetos do computador do computador na nuvem sejam sincronizados com o Azure AD. A sincronização de dispositivos do Azure AD deve ser habilitada e sincronizada nos últimos 60 minutos.|
|azureAdDeviceSyncCheckLongSyncCircle|A verificação se o objeto do computador do computador na nuvem foi sincronizado com Azure Active Directory (Azure AD) foi o tempo de tempo. Certifique-se de que a conexão do Azure AD funcione e sincronize com frequência para que os objetos do computador do computador na nuvem sejam sincronizados com o Azure AD. A sincronização de dispositivos do Azure AD deve ser habilitada e sincronizada nos últimos 60 minutos.|
|azureAdDeviceSyncCheckUnknownError|Falha na Azure Active Directory de conectividade híbrida (Azure AD). Certifique-se de que a conexão do Azure AD funcione e sincronize com frequência para que os objetos do computador do computador na nuvem sejam sincronizados com o Azure AD. A sincronização de dispositivos do Azure AD deve ser habilitada e sincronizada nos últimos 60 minutos.|
|resourceAvailabilityCheckNoSubnetIP|A sub-rede fornecida não tem endereços IP disponíveis. Verifique se a sub-rede fornecida na conexão de rede local tem endereços IP suficientes disponíveis. Expanda a sub-rede selecionada atual ou selecione uma sub-rede diferente a ser usada para provisionamento.|
|resourceAvailabilityCheckSubscriptionDisabled|A assinatura do Azure fornecida está desabilitada. Verifique se a assinatura do Azure está habilitada e disponível para provisionamento.|
|resourceAvailabilityCheckAzurePolicyViolation|A assinatura do Azure fornecida não pode ser encontrada. Verifique se a assinatura do Azure está disponível para provisionamento.|
|resourceAvailabilityCheckSubscriptionNotFound|A assinatura do Azure fornecida não pode ser acessada. Verifique se a assinatura do Azure está disponível para provisionamento.|
|resourceAvailabilityCheckSubscriptionTransferred|A assinatura do Azure fornecida não pode ser acessada. Verifique se a assinatura do Azure está disponível para provisionamento.|
|resourceAvailabilityCheckGeneralSubscriptionError|Uma política do Azure está restringindo a criação de recursos. Verifique se não há nenhuma política do Azure que restrinja a criação de recursos no grupo de assinaturas e/ou recursos.|
|resourceAvailabilityCheckUnsupportedVNetRegion|O vNet selecionado está localizado em uma região sem suporte. Verifique se o vNet selecionado está localizado em uma região com suporte.|
|resourceAvailabilityCheckUnknownError|A verificação de disponibilidade de recursos do Azure falhou devido a um erro desconhecido. Verifique se todos os recursos do Azure atendem aos pré-requisitos.|
|permissionCheckNoSubscriptionReaderRole|A entidade de serviço de computador na nuvem não tem permissões suficientes na assinatura do Azure. Certifique-se de que a entidade de serviço do computador na nuvem tenha as *permissões Reader* na assinatura.|
|permissionCheckNoResourceGroupOwnerRole|A entidade de serviço de computador na nuvem não tem permissões suficientes no grupo de recursos do Azure. Verifique se a entidade de serviço do computador na nuvem tem as *permissões Owner* no grupo de recursos. |
|permissionCheckNoVNetContributorRole|A entidade de serviço de computador na nuvem não tem permissões suficientes na vNet do Azure. Verifique se o serviço de computador na nuvem tem as *permissões do* colaborador de rede na vNet.|
|permissionCheckNoResourceGroupNetworkContributorRole|A entidade de serviço de computador na nuvem não tem permissões suficientes no grupo de recursos do Azure. Verifique se o aplicativo tem permissões de colaboradores de rede no grupo de recursos.|
|permissionCheckUnknownError|A entidade de serviço de computador na nuvem não tem permissões suficientes. Verifique se a entidade de serviço do computador na nuvem recebe permissões suficientes do Azure.|
|internalServerErrorDeploymentCanceled|A implantação foi cancelada. Tente novamente mais tarde. Se o problema persistir, entre em contato com o suporte.|
|internalServerErrorAllocateResourceFailed|A alocação de recursos falhou. Tente novamente mais tarde. Se o problema persistir, entre em contato com o suporte.|
|internalServerErrorVMDeploymentTimeout|O tempo de implantação da máquina virtual foi o tempo de implantação. Tente novamente mais tarde. Se o problema persistir, entre em contato com o suporte.|
|internalServerErrorUnableToRunDscScript|Durante o provisionamento, alguns scripts DSC do PowerShell são executados no computador de nuvem. Não é possível baixar esses scripts DSC ou executá-los durante a verificação de saúde. Verifique se a vNet tem acesso irrestrito aos pontos de extremidade necessários, e o PowerShell não está bloqueado no ambiente ou na Política de Grupo.|
|internalServerUnknownError|O provisionamento falhou devido a um erro interno. Entre em contato com o suporte ao cliente.|

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
