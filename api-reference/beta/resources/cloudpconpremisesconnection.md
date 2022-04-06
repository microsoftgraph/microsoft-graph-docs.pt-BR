---
title: Tipo de recurso cloudPcOnPremisesConnection
description: Representa uma coleção definida de informações de recursos do Azure que podem ser usadas para estabelecer a conectividade de rede local para PCs na Nuvem.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: d849bb6b2d5666e0e9953d4684bf20596bf938ff
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587284"
---
# <a name="cloudpconpremisesconnection-resource-type"></a>Tipo de recurso cloudPcOnPremisesConnection

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção definida de informações de recursos do Azure que podem ser usadas para estabelecer a conectividade de rede local para PCs na Nuvem.

[!INCLUDE [on-premise-rename-note](../../includes/on-premise-rename-note.md)]

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[Coleção cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Listar propriedades e relações dos objetos [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Obter cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-get.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Leia as propriedades e as relações do [objeto cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Criar cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Crie um novo [objeto cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Atualizar cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-update.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Atualize as propriedades de [um objeto cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Excluir cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-delete.md)|Nenhum|[Exclua um objeto cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md). Você não pode excluir uma conexão que está em uso.|
|[RunHealthChecks de cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Nenhum|Execute verificações de saúde na [nuvemPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).|
|[updateAdDomainPassword](../api/cloudpconpremisesconnection-updateaddomainpassword.md)|Nenhum|Atualize a senha de domínio do Active Directory para uma [nuvem bem-sucedidaPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md). Essa API é suportada quando o tipo do **onPremisesConnection** é `hybridAzureADJoin`.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para a conexão de rede do Azure. Somente leitura.|
|managedBy|[cloudPcManagementService](#cloudpcmanagementservice-values)|Especifica quais serviços gerenciam a conexão local. Os valores possíveis são: `windows365`e `devBox` `unknownFutureValue`. Somente leitura.
|type|[cloudPcOnPremisesConnectionType](#cloudpconpremisesconnectiontype-values)|Especifica como o Cloud PC provisionado será ingressado no Azure Active Directory. O valor padrão é `hybridAzureADJoin`. Os valores possíveis são: `azureADJoin`, `hybridAzureADJoin`, `unknownFutureValue`.|
|displayName|Cadeia de caracteres|O nome de exibição da conexão de rede do Azure.|
|subscriptionId|Cadeia de caracteres|A ID da assinatura de destino do Azure associada ao seu locatário.|
|subscriptionName|String|O nome da assinatura de destino do Azure. Somente leitura.|
|adDomainName|String|O FQDN (nome de domínio totalmente qualificado) do domínio do Active Directory que você deseja ingressar. Opcional.|
|adDomainUsername|Cadeia de caracteres|O nome de usuário de uma conta do Active Directory (conta de usuário ou serviço) que tem permissões para criar objetos de computador no Active Directory. Formato obrigatório: admin@contoso.com. Opcional.|
|adDomainPassword|String|A senha associada **a adDomainUsername**.|
|organizationalUnit|Cadeia de caracteres|A unidade organizacional (OU) na qual a conta do computador é criada. Se deixado nulo, a UO configurada como padrão (um contêiner de objeto de computador conhecido) em seu domínio do Active Directory (OU) será usada. Opcional.|
|resourceGroupId|Cadeia de caracteres|A ID do grupo de recursos de destino. Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".|
|virtualNetworkId|Cadeia de caracteres|A ID da rede virtual de destino. Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".|
|subnetId|Cadeia de caracteres|A ID da sub-rede de destino. Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".|
|healthCheckStatus|[cloudPcOnPremisesConnectionStatus](#cloudpconpremisesconnectionstatus-values)|O status da verificação de saúde mais recente feita na conexão de rede do Azure. Por exemplo, se o status for "passado", a conexão de rede do Azure passou todas as verificações executados pelo serviço. Os valores possíveis são: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`. Somente leitura.|
|healthCheckStatusDetails|[cloudPcOnPremisesConnectionStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md)|Os detalhes das verificações de saúde da conexão e os resultados correspondentes. Retornado somente em `$select`. Para obter um exemplo que mostra como obter a propriedade **inUse** , consulte o Exemplo 2: Obter as propriedades selecionadas de uma conexão de rede do [Azure, incluindo healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md). Somente leitura.|
|inUse|Booliano|Quando `true`, a conexão de rede do Azure está em uso. Quando `false`, a conexão não está em uso. Não é possível excluir uma conexão que está em uso. Retornado apenas em `$select`. Para obter um exemplo que mostra como obter a propriedade **inUse** , consulte o Exemplo 2: Obter as propriedades selecionadas de uma conexão de rede do [Azure, incluindo healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md). Somente leitura.|

### <a name="cloudpcmanagementservice-values"></a>Valores do cloudPcManagementService

|Membro| Valor |Descrição|
|:---|:---|:---|
|windows365|1| A conexão local foi criada com êxito por meio do Windows365.|
|devBox|2| A conexão local foi criada com êxito por meio Project Fidalgo.|
|unknownFutureValue|4| Valor de sentinela de enumeração evolvável. Não usar.|

### <a name="cloudpconpremisesconnectiontype-values"></a>valores cloudPcOnPremisesConnectionType

|Member|Descrição|
|:---|:---|
|hybridAzureADJoin|Ingressou no Active Directory local e no Azure AD. Somente usuários híbridos podem ser atribuídos e entrar no Cloud PC.|
|azureADJoin|Ingresse apenas no Azure AD. Usuários híbridos e somente na nuvem podem ser atribuídos e entrar no Cloud PC.|
|unknownFutureValue|Valor de sentinela de enumeração evolvável. Não usar.|

### <a name="cloudpconpremisesconnectionstatus-values"></a>valores cloudPcOnPremisesConnectionStatus

|Member|Descrição|
|:---|:---|
|pendente|Criado e aguardando verificações de saúde.|
|running|Verificações de saúde estão em execução.|
|passado|Verificações de saúde passadas.|
|failed|Falha nas verificações de saúde.|
|warning|Verificações de saúde passadas com aviso.|
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
  "managedBy": "String",
  "type": "String",
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
