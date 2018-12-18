---
title: tipo de recurso de androidPermissionAction
description: Mapeamento entre uma permissão de app Android e a ação Android deve ser adotada quando essa permissão é solicitada.
author: tfitzmac
ms.openlocfilehash: 90117b30dae765151e79d8ad1c2ae1afaa5a42ff
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331133"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="ebebc-103">tipo de recurso de androidPermissionAction</span><span class="sxs-lookup"><span data-stu-id="ebebc-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="ebebc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ebebc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebebc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ebebc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebebc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ebebc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebebc-107">Mapeamento entre uma permissão de app Android e a ação Android deve ser adotada quando essa permissão é solicitada.</span><span class="sxs-lookup"><span data-stu-id="ebebc-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>
## <a name="properties"></a><span data-ttu-id="ebebc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ebebc-108">Properties</span></span>
|<span data-ttu-id="ebebc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebebc-109">Property</span></span>|<span data-ttu-id="ebebc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebebc-110">Type</span></span>|<span data-ttu-id="ebebc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebebc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebebc-112">permissão</span><span class="sxs-lookup"><span data-stu-id="ebebc-112">permission</span></span>|<span data-ttu-id="ebebc-113">String</span><span class="sxs-lookup"><span data-stu-id="ebebc-113">String</span></span>|<span data-ttu-id="ebebc-114">String de permissão Android, definido na documentação oficial Android.</span><span class="sxs-lookup"><span data-stu-id="ebebc-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="ebebc-115">Exemplo 'android.permission.READ_CONTACTS'.</span><span class="sxs-lookup"><span data-stu-id="ebebc-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="ebebc-116">action</span><span class="sxs-lookup"><span data-stu-id="ebebc-116">action</span></span>|[<span data-ttu-id="ebebc-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="ebebc-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="ebebc-118">Tipo de ação de permissão Android.</span><span class="sxs-lookup"><span data-stu-id="ebebc-118">Type of Android permission action.</span></span> <span data-ttu-id="ebebc-119">Os valores possíveis são: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="ebebc-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebebc-120">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="ebebc-120">Relationships</span></span>
<span data-ttu-id="ebebc-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ebebc-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ebebc-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ebebc-122">JSON Representation</span></span>
<span data-ttu-id="ebebc-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ebebc-123">Here is a JSON representation of the resource.</span></span>
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





