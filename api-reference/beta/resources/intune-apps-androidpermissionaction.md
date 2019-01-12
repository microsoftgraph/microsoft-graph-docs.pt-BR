---
title: tipo de recurso de androidPermissionAction
description: Mapeamento entre uma permissão de app Android e a ação Android deve ser adotada quando essa permissão é solicitada.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5ad7b438951b947cc515f1472dd1eae8caf472f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977119"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="8b4c4-103">tipo de recurso de androidPermissionAction</span><span class="sxs-lookup"><span data-stu-id="8b4c4-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="8b4c4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8b4c4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b4c4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8b4c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b4c4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8b4c4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b4c4-107">Mapeamento entre uma permissão de app Android e a ação Android deve ser adotada quando essa permissão é solicitada.</span><span class="sxs-lookup"><span data-stu-id="8b4c4-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>
## <a name="properties"></a><span data-ttu-id="8b4c4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b4c4-108">Properties</span></span>
|<span data-ttu-id="8b4c4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b4c4-109">Property</span></span>|<span data-ttu-id="8b4c4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b4c4-110">Type</span></span>|<span data-ttu-id="8b4c4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b4c4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b4c4-112">permissão</span><span class="sxs-lookup"><span data-stu-id="8b4c4-112">permission</span></span>|<span data-ttu-id="8b4c4-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b4c4-113">String</span></span>|<span data-ttu-id="8b4c4-114">String de permissão Android, definido na documentação oficial Android.</span><span class="sxs-lookup"><span data-stu-id="8b4c4-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="8b4c4-115">Exemplo 'android.permission.READ_CONTACTS'.</span><span class="sxs-lookup"><span data-stu-id="8b4c4-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="8b4c4-116">action</span><span class="sxs-lookup"><span data-stu-id="8b4c4-116">action</span></span>|[<span data-ttu-id="8b4c4-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="8b4c4-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="8b4c4-118">Tipo de ação de permissão Android.</span><span class="sxs-lookup"><span data-stu-id="8b4c4-118">Type of Android permission action.</span></span> <span data-ttu-id="8b4c4-119">Os valores possíveis são: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="8b4c4-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b4c4-120">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="8b4c4-120">Relationships</span></span>
<span data-ttu-id="8b4c4-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8b4c4-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8b4c4-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b4c4-122">JSON Representation</span></span>
<span data-ttu-id="8b4c4-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b4c4-123">Here is a JSON representation of the resource.</span></span>
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





