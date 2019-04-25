---
title: tipo de recurso androidPermissionAction
description: O mapeamento entre uma permissão de aplicativo Android e a ação que o Android deve executar quando essa permissão é solicitada.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fec33b2600e88e6a4dfae644c335d9652c20abe0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552349"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="94b27-103">tipo de recurso androidPermissionAction</span><span class="sxs-lookup"><span data-stu-id="94b27-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="94b27-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94b27-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94b27-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94b27-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94b27-106">O mapeamento entre uma permissão de aplicativo Android e a ação que o Android deve executar quando essa permissão é solicitada.</span><span class="sxs-lookup"><span data-stu-id="94b27-106">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="94b27-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94b27-107">Properties</span></span>
|<span data-ttu-id="94b27-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94b27-108">Property</span></span>|<span data-ttu-id="94b27-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="94b27-109">Type</span></span>|<span data-ttu-id="94b27-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="94b27-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94b27-111">autorização</span><span class="sxs-lookup"><span data-stu-id="94b27-111">permission</span></span>|<span data-ttu-id="94b27-112">String</span><span class="sxs-lookup"><span data-stu-id="94b27-112">String</span></span>|<span data-ttu-id="94b27-113">Cadeia de caracteres de permissão Android, definida na documentação oficial do Android.</span><span class="sxs-lookup"><span data-stu-id="94b27-113">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="94b27-114">Exemplo ' Android. Permission. READ_CONTACTS '.</span><span class="sxs-lookup"><span data-stu-id="94b27-114">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="94b27-115">ação</span><span class="sxs-lookup"><span data-stu-id="94b27-115">action</span></span>|[<span data-ttu-id="94b27-116">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="94b27-116">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="94b27-117">Tipo de ação de permissão de Android.</span><span class="sxs-lookup"><span data-stu-id="94b27-117">Type of Android permission action.</span></span> <span data-ttu-id="94b27-118">Os valores possíveis são: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="94b27-118">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94b27-119">Relações</span><span class="sxs-lookup"><span data-stu-id="94b27-119">Relationships</span></span>
<span data-ttu-id="94b27-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94b27-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94b27-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94b27-121">JSON Representation</span></span>
<span data-ttu-id="94b27-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94b27-122">Here is a JSON representation of the resource.</span></span>
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





