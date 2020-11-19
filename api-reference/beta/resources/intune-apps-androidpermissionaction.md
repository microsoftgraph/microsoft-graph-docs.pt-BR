---
title: tipo de recurso androidPermissionAction
description: O mapeamento entre uma permissão de aplicativo Android e a ação que o Android deve executar quando essa permissão é solicitada.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76090d450332b0c5656ee122a7338180fa692811
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49231917"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="4a66a-103">tipo de recurso androidPermissionAction</span><span class="sxs-lookup"><span data-stu-id="4a66a-103">androidPermissionAction resource type</span></span>

<span data-ttu-id="4a66a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a66a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a66a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4a66a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a66a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a66a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a66a-107">O mapeamento entre uma permissão de aplicativo Android e a ação que o Android deve executar quando essa permissão é solicitada.</span><span class="sxs-lookup"><span data-stu-id="4a66a-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="4a66a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a66a-108">Properties</span></span>
|<span data-ttu-id="4a66a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a66a-109">Property</span></span>|<span data-ttu-id="4a66a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a66a-110">Type</span></span>|<span data-ttu-id="4a66a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a66a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a66a-112">autorização</span><span class="sxs-lookup"><span data-stu-id="4a66a-112">permission</span></span>|<span data-ttu-id="4a66a-113">String</span><span class="sxs-lookup"><span data-stu-id="4a66a-113">String</span></span>|<span data-ttu-id="4a66a-114">Cadeia de caracteres de permissão Android, definida na documentação oficial do Android.</span><span class="sxs-lookup"><span data-stu-id="4a66a-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="4a66a-115">Exemplo ' android.permission.READ_CONTACTS '.</span><span class="sxs-lookup"><span data-stu-id="4a66a-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="4a66a-116">ação</span><span class="sxs-lookup"><span data-stu-id="4a66a-116">action</span></span>|[<span data-ttu-id="4a66a-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="4a66a-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="4a66a-118">Tipo de ação de permissão de Android.</span><span class="sxs-lookup"><span data-stu-id="4a66a-118">Type of Android permission action.</span></span> <span data-ttu-id="4a66a-119">Os valores possíveis são: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="4a66a-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a66a-120">Relações</span><span class="sxs-lookup"><span data-stu-id="4a66a-120">Relationships</span></span>
<span data-ttu-id="4a66a-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a66a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a66a-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a66a-122">JSON Representation</span></span>
<span data-ttu-id="4a66a-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a66a-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidPermissionAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidPermissionAction",
  "permission": "String",
  "action": "String"
}
```




