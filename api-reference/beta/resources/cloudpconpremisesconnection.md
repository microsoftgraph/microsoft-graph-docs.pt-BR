---
title: Tipo de recurso cloudPcOnPremisesConnection
description: Representa uma coleção definida de informações de recursos do Azure que podem ser usadas para estabelecer a conectividade de rede local para PCs na nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 00b129ed73b64ed9ac0785017cfad8c2a74fde2b
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50033992"
---
# <a name="cloudpconpremisesconnection-resource-type"></a>Tipo de recurso cloudPcOnPremisesConnection

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção definida de informações de recursos do Azure que podem ser usadas para estabelecer a conectividade de rede local para PCs na nuvem.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[Coleção cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Listar propriedades e relações dos objetos [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Obter cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-get.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Leia as propriedades e os relacionamentos do objeto [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Criar cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Crie um novo [objeto cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Atualizar cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-update.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Atualizar as propriedades de um [objeto cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Excluir cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-delete.md)|Nenhum|[Exclua um objeto cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md) Não é possível excluir uma conexão que está em uso.|
|[RunHealthChecks of cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Nenhum|Execute verificações de saúde na [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).|
|[updateAdDomainPassword](../api/cloudpconpremisesconnection-updateaddomainpassword.md)|Nenhum|Atualize a senha do domínio do AD para uma [cloudPcOnPremisesConnection bem-sucedida.](../resources/cloudpconpremisesconnection.md)|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da conexão local. Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição da conexão local.|
|subscriptionId|Cadeia de caracteres|A ID da assinatura do Azure de destino que está associada ao seu locatário.|
|subscriptionName|Cadeia de caracteres|O nome da assinatura do Azure de destino. Somente leitura.|
|adDomainName|Cadeia de caracteres|O nome de domínio totalmente qualificado (FQDN) do domínio do Active Directory no qual você deseja ingressar.|
|adDomainUsername|Cadeia de caracteres|O nome de usuário de uma conta do Active Directory (usuário ou conta de serviço) que tem permissões para criar objetos de computador no Active Directory. Formato obrigatório: admin@contoso.com.|
|adDomainPassword|Cadeia de caracteres|A senha associada a adDomainUsername.|
|organizationalUnit|Cadeia de caracteres|A unidade organizacional (OU) na qual a conta do computador é criada. Se for deixado nulo, a UO configurada como padrão (um contêiner de objeto de computador conhecido) em seu domínio (OU) do Active Directory será usada. Opcional.|
|resourceGroupId|Cadeia de caracteres|A ID do grupo de recursos de destino. Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".|
|virtualNetworkId|Cadeia de caracteres|A ID da rede virtual de destino. Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".|
|subnetId|Cadeia de caracteres|A ID da sub-rede de destino. Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".|
|healthCheckStatus|[cloudPcOnPremisesConnectionStatus](#cloudpconpremisesconnectionstatus-values)|O status da verificação de saúde mais recente feita na conexão local. Por exemplo, se o status for "passado", a conexão local passou em todas as verificações que são executados pelo serviço. Os valores possíveis são: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`. Somente leitura.|
|healthCheckStatusDetails|[cloudPcOnPremisesConnectionStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md)|Os detalhes das verificações de saúde da conexão e os resultados correspondentes. Retornado apenas em `$select`. Veja um [exemplo de](../api/cloudpconpremisesconnection-get.md) como obter a propriedade healthCheckStatusDetails. Somente leitura.|
|inUse|Boolean|Quando verdadeiro, a conexão local está em uso. Quando falso, a conexão não está em uso. Não é possível excluir uma conexão que está em uso. Somente leitura.|

### <a name="cloudpconpremisesconnectionstatus-values"></a>Valores de cloudPcOnPremisesConnectionStatus

|Member|Descrição|
|:---|:---|
|pendente|Criado e aguardando verificações de saúde.
|executando|As verificações de saúde estão em execução.|
|aprovado|Verificações de saúde aprovadas.|
|failed|Falhas nas verificações de saúde.|
|unknownFutureValue|Status futuro desconhecido (reservado, não usado no momento).|

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
