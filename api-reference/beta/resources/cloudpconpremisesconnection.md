---
title: tipo de recurso cloudPcOnPremisesConnection
description: Representa uma coleção definida de informações de recursos do Azure que podem ser usadas para estabelecer conectividade de rede local para PCs em nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a8ac0dea68aaac8c1f720948041cfd1eddc048f6
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378227"
---
# <a name="cloudpconpremisesconnection-resource-type"></a>tipo de recurso cloudPcOnPremisesConnection

Namespace: microsoft.graph

Representa uma coleção definida de informações de recursos do Azure que podem ser usadas para estabelecer conectividade de rede local para PCs em nuvem.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|coleção [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Listar Propriedades e relações dos objetos [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Obter cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-get.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Leia as propriedades e as relações do objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Criar cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Criar um novo objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Atualizar cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-update.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Atualiza as propriedades de um objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Excluir cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-delete.md)|Nenhum|Excluir um objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) . Não é possível excluir uma conexão que está sendo usada.|
|[RunHealthChecks do cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Nenhum|Executar verificações de integridade no [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para a conexão local. Somente leitura.|
|displayName|String|O nome de exibição para a conexão local.|
|subscriptionId|Cadeia de Caracteres|A ID da assinatura de destino do Azure que está associada ao seu locatário.|
|subscriptionname|Cadeia de Caracteres|O nome da assinatura de destino do Azure. Somente leitura.|
|adDomainName|Cadeia de Caracteres|O FQDN (nome de domínio totalmente qualificado) do domínio do Active Directory que você deseja ingressar.|
|adDomainUsername|Cadeia de Caracteres|O nome de usuário de uma conta do Active Directory (usuário ou conta de serviço) que tem permissões para criar objetos de computador no Active Directory. Formato obrigatório: contoso@microsoft.com.|
|adDomainPassword|Cadeia de Caracteres|A senha associada ao adDomainUsername.|
|organizationalUnit|Cadeia de Caracteres|A unidade organizacional (OU) em que a conta de computador é criada. Se for Left NULL, a UO configurada como padrão (um contêiner de objeto de computador conhecido) no seu domínio do Active Directory (OU) será usada. Opcional.|
|resourceGroupId|Cadeia de Caracteres|A ID do grupo de recursos de destino. Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".|
|virtualNetworkId|Cadeia de Caracteres|A ID da rede virtual de destino. Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".|
|subnetid|Cadeia de Caracteres|A ID da sub-rede de destino. Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".|
|healthCheckStatus|cloudPcOnPremisesConnectionStatus|O status da verificação de integridade mais recente feita na conexão local. Por exemplo, se o status for "Passed", a conexão local passará por todas as verificações executadas pelo serviço. Somente leitura. Os valores possíveis são: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.|
|healthCheckStatusDetails|[cloudPcOnPremisesConnectionStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md)|Os detalhes das verificações de integridade da conexão e os resultados correspondentes. Retornado apenas em `$select`. Veja um [exemplo](../api/cloudpconpremisesconnection-get.md) de como obter a propriedade healthCheckStatusDetails. Somente leitura.|
|inUse|Boolean|Quando true, a conexão local está em uso. Quando for false, a conexão não será usada. Você não pode excluir uma conexão que está sendo usada. Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection",
  "baseType": "microsoft.graph.entity",
  "openType": false,
  "optionalProperties": ["healthCheckStatusDetails"]
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
  "id": "String (identifier)",
  "displayName": "String",
  "subscriptionId": "String",
  "subscriptionName": "String",
  "adDomainName": "String",
  "adDomainUsername": "String",
  "adDomainPassword": "String",
  "organizationalUnit": "String",
  "resourceGroupId": "String",
  "virtualNetworkId": "String",
  "subnetId": "String",
  "healthCheckStatus": "string",
  "healthCheckStatusDetails": {
    "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionStatusDetails",
    "startDateTime": "String (timestamp)",
    "endDateTime": "String (timestamp)",
    "healthChecks": [
      {
        "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
        "displayName": "String",
        "status": "String",
        "startDateTime": "String (timestamp)",
        "endDateTime": "String (timestamp)",
        "errorType": "String",
        "recommendedAction": "String",
        "additionalDetails": "String"
      }
    ]
  },
  "inUse": "Boolean"
}
```
