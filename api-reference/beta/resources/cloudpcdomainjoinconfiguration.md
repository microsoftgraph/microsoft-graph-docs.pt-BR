---
title: Tipo de recurso cloudPcDomainJoinConfiguration
description: Representa uma configuração definida de como um dispositivo cloud pc provisionado será ingressado no Azure Active Directory.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7bb82c080ce1987bba8d0e9dafe9ba2fc49e16a1
ms.sourcegitcommit: c00c61ce35a6f204a9907aa6f2644ea7a86a5b6e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2021
ms.locfileid: "60805534"
---
# <a name="cloudpcdomainjoinconfiguration-resource-type"></a>Tipo de recurso cloudPcDomainJoinConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma configuração definida de como um dispositivo cloud pc provisionado será ingressado no Azure Active Directory (Azure AD).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|onPremisesConnectionId|Cadeia de caracteres|A ID de conexão local que corresponde aos administradores de IT de rede virtual deseja que a política de provisionamento seja usada ao criar PCs na Nuvem. Você pode usar essa propriedade em ambos os tipos de ingresso no domínio: ingressou no _Azure AD_ ou ingressou _no Azure AD híbrido._ Se você inserir um **onPremisesConnectionId,** deixe **regionName** como vazia.|
|regionName|Cadeia de caracteres|A região com suporte do Azure em que o administrador de IT deseja que a política de provisionamento crie PCs na Nuvem. A rede virtual subjacente será criada e gerenciada pelo serviço Windows 365. Isso só poderá ser inserido se o administrador de IT escolher o Azure AD ingressado como o tipo de ingresso no domínio. Se você inserir um **regionName,** deixe **onPremisesConnectionId** como vazio.|
|type|[cloudPcDomainJoinType](#cloudpcdomainjointype-values)|Especifica como o cloud pc provisionado será ingressado no Azure AD. Se você escolher o tipo, forneça apenas um valor para `hybridAzureADJoin` a **propriedade onPremisesConnectionId** e deixe **regionName** como vazia. Se você escolher o tipo, forneça um `azureADJoin` valor para **onPremisesConnectionId** ou **regionName**. Os valores possíveis são: `azureADJoin`, `hybridAzureADJoin`, `unknownFutureValue`.|

### <a name="cloudpcdomainjointype-values"></a>valores cloudPcDomainJoinType

|Member|Descrição|
|:---|:---|
|azureADJoin|Ingresse apenas no Azure AD. Usuários híbridos e somente na nuvem podem ser atribuídos e entrar no Cloud PC.|
|hybridAzureADJoin|Ingressado no AD local e no Azure AD. Somente usuários híbridos podem ser atribuídos e entrar no Cloud PC.|
|unknownFutureValue|Valor de sentinela de enumeração evolvável. Não usar.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcDomainJoinConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcDomainJoinConfiguration",
  "type": "String",
  "regionName": "String",
  "onPremisesConnectionId": "String"
}
```
