---
title: Tipo de recurso cloudPcOnPremisesConnectionHealthCheck
description: O resultado de uma verificação de saúde de conexão local do computador na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: adc215b32635476320913b2d14aac33ec6ccfc95
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241146"
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
|adJoinCheckOrganizationalUnitIncorrectFormat|A verificação de junção de domínio ativo falhou ao usar o formato da unidade organizacional especificada está incorreta. Formato de exemplo: "OU=OU1,OU=OU2,OU=OU3,DC=DC1".|
|adJoinCheckAccessDenied|A verificação de junção de domínio ativo falhou porque o acesso é negado quando usuários não administradores que foram delegados tentam ingressar objetos de computador em um controlador de domínio. Atribua a permissão correta ao cliente para ingressar no objeto do computador no domínio. Permissões necessárias: Criar objetos de computador, Excluir objetos do computador.|
|adJoinCheckUnknownError|A verificação de junção de domínio ativo falhou devido a um erro desconhecido. Entre em contato com o suporte ao cliente.|
|endpointConnectivityCheckUrlNotWhitelisted|A verificação de conectividade do ponto de extremidade falhou porque as URLs não estão na lista de permitir nas configurações de firewall de rede. Adicione as URLs à lista de autorizações para as configurações de firewall de rede. Consulte [a lista de URL necessárias para](/azure/virtual-desktop/safe-url-list) obter informações de URL.|
|endpointConnectivityCheckUnknownError|A verificação de conectividade do ponto de extremidade falhou devido a um erro desconhecido. Entre em contato com o suporte ao cliente.|
|aadConnectivityCheckUnknownError|A Azure Active Directory de conectividade falhou devido a um erro desconhecido. Entre em contato com o suporte ao cliente.|
|resourceAvailabilityCheckNoSubnetIP|A verificação de disponibilidade do recurso falhou porque não havia endereços IP disponíveis na sub-rede. Free up some or change to another subnet and retry.|
|resourceAvailabilityCheckSubscriptionDisabled|A verificação de disponibilidade do recurso falhou devido a uma assinatura desabilitada do Azure. Reabilitar a assinatura.|
|resourceAvailabilityCheckUnknownError|A verificação de disponibilidade do recurso falhou devido a um erro desconhecido. Entre em contato com o suporte ao cliente.|
|permissionCheckNoSubscriptionReaderRole|Cloud PC de serviço não tem permissões de leitor na assinatura especificada do Azure. Trabalhe com o proprietário da assinatura para adicionar a atribuição de função de leitor na assinatura do Azure para a entidade Cloud PC serviço.|
|permissionCheckNoResourceGroupOwnerRole|Cloud PC de serviço não tem permissões de proprietário no grupo de recursos especificado. Trabalhe com o proprietário da assinatura para adicionar atribuição de função de proprietário no grupo de recursos da entidade Cloud PC de serviço.|
|permissionCheckNoVNetContributorRole|Cloud PC de serviço não tem permissões de colaborador de rede na rede virtual especificada. Trabalhe com o proprietário da assinatura para adicionar a atribuição de função de colaborador de rede para a entidade Cloud PC de serviço. |
|permissionCheckUnknownError|A verificação de permissão falhou devido a um erro desconhecido. Entre em contato com o suporte ao cliente.|
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
