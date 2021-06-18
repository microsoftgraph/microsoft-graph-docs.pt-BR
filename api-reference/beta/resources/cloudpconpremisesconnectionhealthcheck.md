---
title: Tipo de recurso cloudPcOnPremisesConnectionHealthCheck
description: O resultado de uma verificação de saúde de conexão local do computador na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 0323ee64056df1019cc2a8f6e2bd004ffec223b7
ms.sourcegitcommit: 2d0daa446c7b37ced1d214e0c6e18e2b8243bb09
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2021
ms.locfileid: "53010196"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>Tipo de recurso cloudPcOnPremisesConnectionHealthCheck

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O resultado de uma verificação de saúde de conexão local do computador na nuvem.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

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
|dnsCheckFqdnNotFound|A verificação DNS falhou porque o nome de domínio totalmente qualificado não foi encontrado. Insira o nome de domínio totalmente qualificado.|
|dnsCheckUnknownError|A verificação DNS falhou devido a um erro desconhecido. Entre em contato com o suporte ao cliente.|
|adJoinCheckFqdnNotFound|A verificação de junção de domínio ativo falhou porque o nome de domínio totalmente qualificado não foi encontrado. Insira o nome de domínio totalmente qualificado.|
|adJoinCheckIncorrectCredentials|A verificação de junção de domínio ativo falhou porque as credenciais de domínio estão incorretas. Atualize o nome de usuário e a senha.|
|adJoinCheckOrganizationalUnitNotFound|A verificação de junção de domínio ativo falhou porque a unidade organizacional especificada não foi encontrada. Insira a unidade de organização de nova.|
|adJoinCheckOrganizationalUnitIncorrectFormat|A verificação de junção de domínio ativo falhou porque o formato da unidade organizacional especificada está incorreto. Formato de exemplo: "OU=OU1,OU=OU2,OU=OU3,DC=DC1".|
|adJoinCheckAccessDenied|A verificação de junção de domínio ativo falhou porque o acesso é negado quando usuários não administradores que foram delegados tentam ingressar objetos de computador em um controlador de domínio. Atribua a permissão correta ao cliente para ingressar no objeto do computador no domínio. Permissões necessárias: Criar objetos de computador, Excluir objetos do computador.|
|adJoinCheckUnknownError|A verificação de junção de domínio ativo falhou devido a um erro desconhecido. Entre em contato com o suporte ao cliente.|
|endpointConnectivityCheckCloudPcUrlNotAllowListed|A verificação de conectividade do ponto de extremidade falhou porque a URL de armazenamento de script de provisionamento de CPC não está na lista de permitir nas configurações de firewall de rede. Adicione URLs à lista de configurações de firewall de rede permitidas. As URLs podem ser encontradas em informações adicionais.|
|endpointConnectivityCheckWVDUrlNotAllowListed|A verificação de conectividade do ponto de extremidade falhou porque a URL do WVD não está na lista de permitir nas configurações de firewall de rede. Adicione URLs à lista de configurações de firewall de rede permitidas.|
|endpointConnectivityCheckIntuneUrlNotAllowListed|A verificação de conectividade do ponto de extremidade falhou porque a URL do Intune não está na lista de permitir nas configurações de firewall de rede. Adicione URLs à lista de configurações de firewall de rede permitidas.|
|endpointConnectivityCheckUnknownError|A verificação de conectividade do ponto de extremidade falhou devido a um erro desconhecido. Entre em contato com o suporte ao cliente.|
|aadConnectivityCheckUnknownError|A Active Directory do Azure de conectividade falhou devido a um erro desconhecido. Entre em contato com o suporte ao cliente.|
|resourceAvailabilityCheckNoSubnetIP|A verificação de disponibilidade do recurso falhou porque não havia endereços IP disponíveis na sub-rede. Free up some or change to another subnet and retry.|
|resourceAvailabilityCheckSubscriptionDisabled|A verificação de disponibilidade do recurso falhou devido a uma assinatura desabilitada do Azure. Reabilitar a assinatura.|
|resourceAvailabilityCheckAzurePolicyViolation|A criação do recurso do Azure necessário falhou porque a política do Azure de suas organizações bloqueou a ação. Atualize sua política do Azure para permitir essa criação de recursos.|
|resourceAvailabilityCheckUnsupportedVNetRegion|O vNet selecionado não está em uma região do Azure com suporte.|
|resourceAvailabilityCheckUnknownError|A verificação de disponibilidade do recurso falhou devido a um erro desconhecido. Entre em contato com o suporte ao cliente.|
|permissionCheckNoSubscriptionReaderRole|A entidade de serviço de computador na nuvem não tem permissões de leitor na assinatura especificada do Azure. Trabalhe com o proprietário da assinatura para adicionar a atribuição de função de leitor na assinatura do Azure para a entidade de serviço do Cloud PC.|
|permissionCheckNoResourceGroupOwnerRole|A entidade de serviço do computador na nuvem não tem permissões de proprietário no grupo de recursos especificado. Trabalhe com o proprietário da assinatura para adicionar a atribuição de função de proprietário no grupo de recursos para a entidade de serviço do Cloud PC.|
|permissionCheckNoVNetContributorRole|A entidade de serviço de computador na nuvem não tem permissões de colaborador de rede na rede virtual especificada. Trabalhe com o proprietário da assinatura para adicionar a atribuição de função de colaborador de rede para a entidade de serviço do Cloud PC. |
|permissionCheckUnknownError|A verificação de permissão falhou devido a um erro desconhecido. Entre em contato com o suporte ao cliente.|
|internalServerErrorDeploymentCanceled|A implantação foi cancelada. Tente novamente mais tarde. Se o problema persistir, contate o suporte.|
|internalServerErrorAllocateResourceFailed|A alocação de recursos falhou. Tente novamente ou contate o suporte para obter mais detalhes.|
|internalServerErrorVMDeploymentTimeout|O tempo de implantação da máquina virtual foi o tempo de implantação. Tentar novamente. Se o problema persistir, contate o suporte.|
|internalServerErrorUnableToRunDscScript|Não é possível executar o script DSC durante a verificação de saúde. O serviço precisa de acesso ao WinRM para provisionar com êxito o computador de nuvem. Verifique se nenhuma Política de Grupo ou configuração relacionada está bloqueando o uso do PowerShell/DSC.|
|internalServerUnknownError|A verificação de saúde falhou devido a um erro de servidor interno desconhecido. Entre em contato com o suporte ao cliente.|

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
