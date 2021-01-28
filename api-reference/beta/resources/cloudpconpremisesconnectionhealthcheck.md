---
title: Tipo de recurso cloudPcOnPremisesConnectionHealthCheck
description: O resultado de uma verificação de saúde de conexão local do computador na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 32b57750400e1fb71dc8cc173b364fba76cd36ec
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50033978"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>Tipo de recurso cloudPcOnPremisesConnectionHealthCheck

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O resultado de uma verificação de saúde de conexão local do computador na nuvem.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[RunHealthChecks of cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Nenhum|Execute as verificações de saúde de [uma cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição deste item de verificação de saúde.|
|status|[cloudPcOnPremisesConnectionStatus](../resources/cloudpconpremisesconnection.md#cloudpconpremisesconnectionstatus-values)|O status do item de verificação de saúde. Os valores possíveis são: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`. Somente leitura.|
|startDateTime|DateTimeOffset|A hora de início do item de verificação de saúde. Somente leitura.|
|endDateTime|DateTimeOffset|A hora de término do item de verificação de saúde. Somente leitura.|
|errorType|[cloudPcOnPremisesConnectionHealthCheckErrorType](#cloudpconpremisesconnectionhealthcheckerrortype-values)|O tipo de erro que ocorreu durante a verificação de saúde.|
|recommendedAction|Cadeia de caracteres|A ação recomendada para corrigir o erro correspondente.|
|additionalDetails|Cadeia de caracteres|Detalhes adicionais sobre a verificação de saúde ou a ação recomendada.|

### <a name="cloudpconpremisesconnectionhealthcheckerrortype-values"></a>Valores de cloudPcOnPremisesConnectionHealthCheckErrorType

|Member|Descrição|
|:---|:---|
|dnsCheckFqdnNotFound|A verificação de DNS falhou porque o nome de domínio totalmente qualificado não foi encontrado. Insira o nome de domínio totalmente qualificado.|
|dnsCheckUnknownError|A verificação de DNS falhou devido a um erro desconhecido. Entre em contato com o suporte ao cliente.|
|adJoinCheckFqdnNotFound|A verificação de junção de domínio ativo falhou porque o nome de domínio totalmente qualificado não foi encontrado. Insira o nome de domínio totalmente qualificado.|
|adJoinCheckIncorrectCredentials|A verificação de participação no domínio ativo falhou porque as credenciais do domínio estão incorretas. Atualize o nome de usuário e a senha.|
|adJoinCheckOrganizationalUnitNotFound|A verificação de junção de domínio ativo falhou porque a unidade organizacional especificada não foi encontrada. Insira a unidade da organização.|
|adJoinCheckOrganizationalUnitIncorrectFormat|A verificação de junção de domínio ativo falhou ao usar o formato da unidade organizacional especificada está incorreto. Formato de exemplo: "OU=OU1,OU=OU2,OU=OU3,DC=DC1".|
|adJoinCheckUnknownError|A verificação de junção de domínio ativo falhou devido a um erro desconhecido. Entre em contato com o suporte ao cliente.|
|endpointConnectivityCheckUrlNotWhitelisted|A verificação de conectividade do ponto de extremidade falhou porque as URLs não estão na lista de autorização nas configurações de firewall da rede. Adicione as URLs à lista de autorizações para as configurações de firewall de rede. Consulte [a lista de URLs necessárias](/azure/virtual-desktop/safe-url-list) para obter informações de URL.|
|endpointConnectivityCheckUnknownError|A verificação de conectividade do ponto de extremidade falhou devido a um erro desconhecido. Entre em contato com o suporte ao cliente.|
|aadConnectivityCheckUnknownError|A verificação de conectividade do Azure Active Directory falhou devido a um erro desconhecido. Entre em contato com o suporte ao cliente.|
|resourceAvailabilityCheckNoSubnetIP|A verificação de disponibilidade do recurso falhou porque não havia endereços IP disponíveis na sub-rede. Free up some or change to another subnet and retry.|
|resourceAvailabilityCheckSubscriptionDisabled|A verificação de disponibilidade do recurso falhou devido a uma assinatura desabilitada do Azure. Habilita a assinatura.|
|resourceAvailabilityCheckUnknownError|A verificação de disponibilidade do recurso falhou devido a um erro desconhecido. Entre em contato com o suporte ao cliente.|
|permissionCheckNoSubscriptionReaderRole|A entidade de serviço de computador na nuvem não tem permissões de leitor na assinatura especificada do Azure. Trabalhe com o proprietário da assinatura para adicionar a atribuição de função de leitor na assinatura do Azure para a entidade de serviço do Cloud PC.|
|permissionCheckNoResourceGroupOwnerRole|A entidade de serviço do cloud PC não tem permissões de proprietário no grupo de recursos especificado. Trabalhe com o proprietário da assinatura para adicionar a atribuição de função de proprietário ao grupo de recursos para a entidade de serviço do Cloud PC.|
|permissionCheckNoVNetContributorRole|A entidade de serviço do cloud PC não tem permissões de colaborador de rede na rede virtual especificada. Trabalhe com o proprietário da assinatura para adicionar a atribuição de função de colaborador de rede para a entidade de serviço do Cloud PC. |
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
