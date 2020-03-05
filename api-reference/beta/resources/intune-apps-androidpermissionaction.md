---
title: tipo de recurso androidPermissionAction
description: O mapeamento entre uma permissão de aplicativo Android e a ação que o Android deve executar quando essa permissão é solicitada.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 52b105c831399b935196254d794bd5da513d19f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42494097"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="302d5-103">tipo de recurso androidPermissionAction</span><span class="sxs-lookup"><span data-stu-id="302d5-103">androidPermissionAction resource type</span></span>

<span data-ttu-id="302d5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="302d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="302d5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="302d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="302d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="302d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="302d5-107">O mapeamento entre uma permissão de aplicativo Android e a ação que o Android deve executar quando essa permissão é solicitada.</span><span class="sxs-lookup"><span data-stu-id="302d5-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="302d5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="302d5-108">Properties</span></span>
|<span data-ttu-id="302d5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="302d5-109">Property</span></span>|<span data-ttu-id="302d5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="302d5-110">Type</span></span>|<span data-ttu-id="302d5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="302d5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="302d5-112">autorização</span><span class="sxs-lookup"><span data-stu-id="302d5-112">permission</span></span>|<span data-ttu-id="302d5-113">String</span><span class="sxs-lookup"><span data-stu-id="302d5-113">String</span></span>|<span data-ttu-id="302d5-114">Cadeia de caracteres de permissão Android, definida na documentação oficial do Android.</span><span class="sxs-lookup"><span data-stu-id="302d5-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="302d5-115">Exemplo ' Android. Permission. READ_CONTACTS '.</span><span class="sxs-lookup"><span data-stu-id="302d5-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="302d5-116">ação</span><span class="sxs-lookup"><span data-stu-id="302d5-116">action</span></span>|[<span data-ttu-id="302d5-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="302d5-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="302d5-118">Tipo de ação de permissão de Android.</span><span class="sxs-lookup"><span data-stu-id="302d5-118">Type of Android permission action.</span></span> <span data-ttu-id="302d5-119">Os valores possíveis são: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="302d5-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="302d5-120">Relações</span><span class="sxs-lookup"><span data-stu-id="302d5-120">Relationships</span></span>
<span data-ttu-id="302d5-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="302d5-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="302d5-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="302d5-122">JSON Representation</span></span>
<span data-ttu-id="302d5-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="302d5-123">Here is a JSON representation of the resource.</span></span>
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



