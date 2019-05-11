---
title: tipo de recurso androidPermissionAction
description: O mapeamento entre uma permissão de aplicativo Android e a ação que o Android deve executar quando essa permissão é solicitada.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4766bb91d5d1cde99a12f5a8e4903451a3ac5aca
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950484"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="336e5-103">tipo de recurso androidPermissionAction</span><span class="sxs-lookup"><span data-stu-id="336e5-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="336e5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="336e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="336e5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="336e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="336e5-106">O mapeamento entre uma permissão de aplicativo Android e a ação que o Android deve executar quando essa permissão é solicitada.</span><span class="sxs-lookup"><span data-stu-id="336e5-106">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="336e5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="336e5-107">Properties</span></span>
|<span data-ttu-id="336e5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="336e5-108">Property</span></span>|<span data-ttu-id="336e5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="336e5-109">Type</span></span>|<span data-ttu-id="336e5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="336e5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="336e5-111">autorização</span><span class="sxs-lookup"><span data-stu-id="336e5-111">permission</span></span>|<span data-ttu-id="336e5-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="336e5-112">String</span></span>|<span data-ttu-id="336e5-113">Cadeia de caracteres de permissão Android, definida na documentação oficial do Android.</span><span class="sxs-lookup"><span data-stu-id="336e5-113">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="336e5-114">Exemplo ' Android. Permission. READ_CONTACTS '.</span><span class="sxs-lookup"><span data-stu-id="336e5-114">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="336e5-115">ação</span><span class="sxs-lookup"><span data-stu-id="336e5-115">action</span></span>|[<span data-ttu-id="336e5-116">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="336e5-116">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="336e5-117">Tipo de ação de permissão de Android.</span><span class="sxs-lookup"><span data-stu-id="336e5-117">Type of Android permission action.</span></span> <span data-ttu-id="336e5-118">Os valores possíveis são: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="336e5-118">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="336e5-119">Relações</span><span class="sxs-lookup"><span data-stu-id="336e5-119">Relationships</span></span>
<span data-ttu-id="336e5-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="336e5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="336e5-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="336e5-121">JSON Representation</span></span>
<span data-ttu-id="336e5-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="336e5-122">Here is a JSON representation of the resource.</span></span>
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




