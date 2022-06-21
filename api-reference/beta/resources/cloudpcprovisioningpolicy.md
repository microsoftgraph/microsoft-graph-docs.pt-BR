---
title: Tipo de recurso cloudPcProvisioningPolicy
description: Representa uma política de provisionamento de PC na nuvem.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 5c9e851bf2a8723507e1eaa84bc014a715908770
ms.sourcegitcommit: da9079132db3261aed80e6fc4b9314d16e0847b3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/21/2022
ms.locfileid: "66186936"
---
# <a name="cloudpcprovisioningpolicy-resource-type"></a>Tipo de recurso cloudPcProvisioningPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política de provisionamento de PC na nuvem.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|[Coleção cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Listar propriedades e relações dos objetos [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Obter cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-get.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Leia as propriedades e as relações de um [objeto cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Criar cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Crie um novo [objeto cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Atualizar cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-update.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Atualize as propriedades de um [objeto cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Excluir cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-delete.md)|Nenhum|[Exclua um objeto cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).|
|[Atribuir cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-assign.md)|Nenhum |Atribua [um cloudPcProvisioningPolicy a](../resources/cloudpcprovisioningpolicy.md) grupos de usuários.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|alternateResourceUrl|Cadeia de caracteres|A URL do recurso alternativo vinculado a essa política de provisionamento. Somente leitura.|
|cloudPcGroupDisplayName|String|O nome de exibição do grupo de PC na nuvem no qual os PCs na nuvem residem. Somente leitura.|
|description|Cadeia de caracteres|A descrição da política de provisionamento.|
|displayName|Cadeia de caracteres|O nome de exibição da política de provisionamento.|
|domainJoinConfiguration|[cloudPcDomainJoinConfiguration](../resources/cloudpcdomainjoinconfiguration.md)|Especifica como os PCs na nuvem ingressarão Azure Active Directory.|
|gracePeriodInHours|Int32|O número de horas de espera antes que ocorra o reprovisionamento/desprovisionamento. Somente leitura.|
|id|Cadeia de caracteres|Identificador exclusivo para a política de provisionamento de PC na nuvem. Somente leitura.|
|imageDisplayName|Cadeia de caracteres|O nome de exibição da imagem do sistema operacional que você está provisionando.|
|imageId|String|A ID da imagem do sistema operacional que você deseja provisionar em PCs na nuvem. O formato de uma imagem de tipo de galeria é: {publisher_offer_sku}. Os valores com suporte para cada um dos parâmetros são os seguintes:<ul><li>publisher: Microsoftwindowsdesktop.</li> <li>oferta: windows-ent-cpc.</li> <li>sku: 21h1-ent-cpc-m365, 21h1-ent-cpc-os, 20h2-ent-cpc-m365, 20h2-ent-cpc-os, 20h1-ent-cpc-m365, 20h1-ent-cpc-os, 19h2-ent-cpc-m365 e 19h2-ent-cpc-os.</li></ul>|
|Imagetype|cloudPcProvisioningPolicyImageType|O tipo de imagem do sistema operacional (personalizada ou galeria) que você deseja provisionar em PCs na nuvem. Os valores possíveis são: `gallery` e `custom`.|
|localAdminEnabled|Booliano|Indica se a opção de administrador local está habilitada. Se a opção de administrador local estiver habilitada, o usuário final poderá ser um administrador do dispositivo pc na nuvem. Somente leitura.|
|Managedby|[cloudPcManagementService](../resources/cloudpconpremisesconnection.md#cloudpcmanagementservice-values)|Especifica quais serviços gerenciam a conexão de rede do Azure. Os valores possíveis são: `windows365`, `devBox`, `unknownFutureValue`. Somente leitura.|
|microsoftManagedDesktop|[microsoftManagedDesktop](../resources/microsoftManagedDesktop.md)|As configurações específicas para o Microsoft Managed Desktop, que permitem que os clientes obtenham uma experiência de dispositivo gerenciado para o PC na nuvem. Antes de habilitar Microsoft Managed Desktop, um administrador deve configurá-lo.|
|onPremisesConnectionId|Cadeia de caracteres|A ID do cloudPcOnPremisesConnection. Para garantir que os PCs na nuvem tenham conectividade de rede e que eles ingressem no domínio, escolha uma conexão com uma rede virtual validada pelo serviço de PC na nuvem.|
|windowsSettings|[cloudPcWindowsSettings](../resources/cloudpcwindowssettings.md)|Configurações Windows específicas a serem configuradas durante a criação de PCs na nuvem para essa política de provisionamento.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[coleção cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md)|Uma coleção definida de atribuições de política de provisionamento. Representa o conjunto de grupos Microsoft 365 e grupos de segurança em Azure AD que têm a política de provisionamento atribuída. Retornado apenas em `$expand`. Veja um [exemplo de](../api/cloudpcprovisioningpolicy-get.md) como obter a relação de atribuições. |

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
  "alternateResourceUrl": "String",
  "cloudPcGroupDisplayName": "String",
  "description": "String",
  "displayName": "String",
  "domainJoinConfiguration": {
    "@odata.type": "microsoft.graph.cloudPcDomainJoinConfiguration"
  },
  "gracePeriodInHours": "Integer",
  "id": "String (identifier)",
  "imageDisplayName": "String",
  "imageId": "String",
  "imageType": "String",
  "localAdminEnabled": "Boolean",
  "managedBy": "String",
  "microsoftManagedDesktop": {
    "type": "String",
    "profile": "String"
  },
  "onPremisesConnectionId": "String",
  "windowsSettings": {
    "@odata.type": "microsoft.graph.cloudPcWindowsSettings"
  }
}
```
