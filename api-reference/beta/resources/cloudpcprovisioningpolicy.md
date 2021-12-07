---
title: Tipo de recurso cloudPcProvisioningPolicy
description: Representa uma política de provisionamento de computador na nuvem.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 64a793151e685e008999b87eeea32dc5e79a7d0a
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322203"
---
# <a name="cloudpcprovisioningpolicy-resource-type"></a>Tipo de recurso cloudPcProvisioningPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política de provisionamento de computador na nuvem.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|[Coleção cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Listar propriedades e relações dos objetos [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Obter cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-get.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Leia as propriedades e as relações de um [objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Criar cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Crie um novo [objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Atualizar cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-update.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Atualize as propriedades de [um objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Excluir cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-delete.md)|Nenhum|[Exclua um objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Atribuir cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-assign.md)|Nenhum |Atribua [um cloudPcProvisioningPolicy a](../resources/cloudpcprovisioningpolicy.md) grupos de usuários.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para a política de provisionamento do Cloud PC. Somente leitura.|
|displayName|String|O nome de exibição da política de provisionamento.|
|description|String|A descrição da política de provisionamento.|
|onPremisesConnectionId|String|A ID do cloudPcOnPremisesConnection. Para garantir que os computadores na nuvem tenham conectividade de rede e que eles participem do domínio, escolha uma conexão com uma rede virtual validada pelo serviço de Computador na Nuvem.|
|imageId|String|A ID da imagem do sistema operacional que você deseja provisionar em PCs na Nuvem. O formato de uma imagem de tipo de galeria é: {publisher_offer_sku}. Os valores com suporte para cada um dos parâmetros são os seguinte:<ul><li>publisher: Microsoftwindowsdesktop.</li> <li>offer: windows-ent-cpc.</li> <li>sku: 21h1-ent-cpc-m365, 21h1-ent-cpc-os, 20h2-ent-cpc-m365, 20h2-ent-cpc-os, 20h1-ent-cpc-m365, 20h1-ent-cpc-os, 19h2-ent-cpc-m365 e 19h2-ent-cpc-os.</li></ul>|
|imageDisplayName|String|O nome de exibição da imagem do sistema operacional que você está provisionando.|
|imageType|cloudPcProvisioningPolicyImageType|O tipo de imagem do sistema operacional (personalizada ou galeria) que você deseja provisionar em PCs na Nuvem. Os valores possíveis são: `gallery` e `custom`.|
|microsoftManagedDesktop|[microsoftManagedDesktop](../resources/microsoftManagedDesktop.md)|As configurações específicas para a Área de Trabalho Gerenciada da Microsoft, que permitem que os clientes recebam uma experiência de dispositivo gerenciado para o cloud pc. Antes de habilitar a Área de Trabalho Gerenciada da Microsoft, um administrador deve configurá-la.|
|domainJoinConfiguration|[cloudPcDomainJoinConfiguration](../resources/cloudpcdomainjoinconfiguration.md)|Especifica como os PCs de Nuvem ingressarão Azure Active Directory.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[coleção cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md)|Uma coleção definida de atribuições de política de provisionamento. Representa o conjunto de Microsoft 365 grupos e grupos de segurança no Azure AD que têm a política de provisionamento atribuída. Retornado apenas em `$expand`. Consulte um [exemplo](../api/cloudpcprovisioningpolicy-get.md) de como obter a relação de atribuições. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "onPremisesConnectionId": "String",
  "imageId": "String",
  "imageDisplayName": "String",
  "imageType": "String",
  "microsoftManagedDesktop": {
    "type": "String",
    "profile": "String"
  },
  "domainJoinConfiguration": {
    "@odata.type": "microsoft.graph.cloudPcDomainJoinConfiguration"
  }
}
```
