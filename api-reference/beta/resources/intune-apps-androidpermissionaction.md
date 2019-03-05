---
title: tipo de recurso androidPermissionAction
description: O mapeamento entre uma permissão de aplicativo Android e a ação que o Android deve executar quando essa permissão é solicitada.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e00bb351f2eff093dee21cb393ba622bc5e29ea9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161569"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="2526c-103">tipo de recurso androidPermissionAction</span><span class="sxs-lookup"><span data-stu-id="2526c-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="2526c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2526c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2526c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2526c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2526c-106">O mapeamento entre uma permissão de aplicativo Android e a ação que o Android deve executar quando essa permissão é solicitada.</span><span class="sxs-lookup"><span data-stu-id="2526c-106">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="2526c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2526c-107">Properties</span></span>
|<span data-ttu-id="2526c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2526c-108">Property</span></span>|<span data-ttu-id="2526c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2526c-109">Type</span></span>|<span data-ttu-id="2526c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2526c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2526c-111">autorização</span><span class="sxs-lookup"><span data-stu-id="2526c-111">permission</span></span>|<span data-ttu-id="2526c-112">String</span><span class="sxs-lookup"><span data-stu-id="2526c-112">String</span></span>|<span data-ttu-id="2526c-113">Cadeia de caracteres de permissão Android, definida na documentação oficial do Android.</span><span class="sxs-lookup"><span data-stu-id="2526c-113">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="2526c-114">Exemplo ' Android. Permission. READ_CONTACTS '.</span><span class="sxs-lookup"><span data-stu-id="2526c-114">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="2526c-115">action</span><span class="sxs-lookup"><span data-stu-id="2526c-115">action</span></span>|[<span data-ttu-id="2526c-116">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="2526c-116">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="2526c-117">Tipo de ação de permissão de Android.</span><span class="sxs-lookup"><span data-stu-id="2526c-117">Type of Android permission action.</span></span> <span data-ttu-id="2526c-118">Os valores possíveis são: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="2526c-118">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2526c-119">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="2526c-119">Relationships</span></span>
<span data-ttu-id="2526c-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2526c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2526c-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2526c-121">JSON Representation</span></span>
<span data-ttu-id="2526c-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2526c-122">Here is a JSON representation of the resource.</span></span>
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




