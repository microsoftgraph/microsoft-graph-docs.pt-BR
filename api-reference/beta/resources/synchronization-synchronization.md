---
title: tipo de recurso de sincronização
description: Representa a funcionalidade para Azure Active Directory sincronização de identidade (Azure AD) por meio da API do Microsoft Graph.
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 9fd52e5fde2a3eee110709d0817930c0a017ee7e
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62226287"
---
# <a name="synchronization-resource-type"></a>tipo de recurso de sincronização

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a funcionalidade para Azure Active Directory sincronização de identidade (Azure AD) por meio da API do Microsoft Graph. A sincronização de identidade (também chamada de *provisionamento*) permite automatizar o provisionamento (criação, manutenção) e o des provisionamento (remoção) de identidades e funções de usuários do Azure AD para aplicativos de nuvem com suporte. Para obter mais informações, consulte [How Application Provisioning works in Azure Active Directory](/azure/active-directory/app-provisioning/how-provisioning-works)

## <a name="methods"></a>Métodos


|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[acquireAccessToken](../api/synchronization-synchronization-acquireaccesstoken.md)|Nenhum| Adquirir um token do OAuth Access para autorizar o serviço de provisionamento do Azure AD para provisionar usuários em um aplicativo. |
|[Adicionar segredos](../api/synchronization-synchronization-secrets.md)|Nenhum| Forneça credenciais para estabelecer conectividade com o sistema de destino. |

<!--
|Method|Return type|Description|
|:---|:---|:---|
|[List synchronizations](../api/synchronization-synchronization-list.md)|[synchronization](../resources/synchronization-synchronization.md) collection|Get a list of the [synchronization](../resources/synchronization-synchronization.md) objects and their properties.|
|[Create synchronization](../api/synchronization-serviceprincipal-post-synchronization.md)|[synchronization](../resources/synchronization-synchronization.md)|Create a new [synchronization](../resources/synchronization-synchronization.md) object.|
|[Get synchronization](../api/synchronization-synchronization-get.md)|[synchronization](../resources/synchronization-synchronization.md)|Read the properties and relationships of a [synchronization](../resources/synchronization-synchronization.md) object.|
|[Update synchronization](../api/synchronization-synchronization-update.md)|[synchronization](../resources/synchronization-synchronization.md)|Update the properties of a [synchronization](../resources/synchronization-synchronization.md) object.|
|[Delete synchronization](../api/synchronization-synchronization-delete.md)|None|Deletes a [synchronization](../resources/synchronization-synchronization.md) object.|
|[Ping](../api/synchronization-synchronization-ping.md)|String|**TODO: Add Description**|
|[acquireAccessToken](../api/synchronization-synchronization-acquireaccesstoken.md)|None|**TODO: Add Description**|
|[List jobs](../api/synchronization-synchronization-list-jobs.md)|[synchronizationJob](../resources/synchronization-synchronizationjob.md) collection|Get the synchronizationJob resources from the jobs navigation property.|
|[Create synchronizationJob](../api/synchronization-synchronization-post-jobs.md)|[synchronizationJob](../resources/synchronization-synchronizationjob.md)|Create a new synchronizationJob object.|
|[List templates](../api/synchronization-synchronization-list-templates.md)|[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) collection|Get the synchronizationTemplate resources from the templates navigation property.|
|[Create synchronizationTemplate](../api/synchronization-synchronization-post-templates.md)|[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)|Create a new synchronizationTemplate object.|
-->

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|secrets|[coleção synchronizationSecretKeyStringValuePair](synchronization-synchronizationsecretkeystringvaluepair.md)| Representa uma coleção de credenciais para acessar aplicativos de nuvem provisionados.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|jobs|[coleção synchronizationJob](../resources/synchronization-synchronizationjob.md)| Executa a sincronização executando periodicamente em segundo plano, sondando alterações em um diretório e empurrando-as para outro diretório.|
|templates|[Coleção synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)| Configurações de sincronização pré-configuradas para um aplicativo específico.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronization",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronization",
  "version": "String",
  "secrets": [
    {
      "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
    }
  ]
}
```

