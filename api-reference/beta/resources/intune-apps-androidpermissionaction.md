---
title: tipo de recurso de androidPermissionAction
description: Mapeamento entre uma permissão de app Android e a ação Android deve ser adotada quando essa permissão é solicitada.
ms.openlocfilehash: e65f9b28169e231e34b5a7a46316821f77639233
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035171"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="bb4a7-103">tipo de recurso de androidPermissionAction</span><span class="sxs-lookup"><span data-stu-id="bb4a7-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="bb4a7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bb4a7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb4a7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bb4a7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb4a7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bb4a7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb4a7-107">Mapeamento entre uma permissão de app Android e a ação Android deve ser adotada quando essa permissão é solicitada.</span><span class="sxs-lookup"><span data-stu-id="bb4a7-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>
## <a name="properties"></a><span data-ttu-id="bb4a7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb4a7-108">Properties</span></span>
|<span data-ttu-id="bb4a7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb4a7-109">Property</span></span>|<span data-ttu-id="bb4a7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb4a7-110">Type</span></span>|<span data-ttu-id="bb4a7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb4a7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb4a7-112">permissão</span><span class="sxs-lookup"><span data-stu-id="bb4a7-112">permission</span></span>|<span data-ttu-id="bb4a7-113">String</span><span class="sxs-lookup"><span data-stu-id="bb4a7-113">String</span></span>|<span data-ttu-id="bb4a7-114">String de permissão Android, definido na documentação oficial Android.</span><span class="sxs-lookup"><span data-stu-id="bb4a7-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="bb4a7-115">Exemplo 'android.permission.READ_CONTACTS'.</span><span class="sxs-lookup"><span data-stu-id="bb4a7-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="bb4a7-116">action</span><span class="sxs-lookup"><span data-stu-id="bb4a7-116">action</span></span>|[<span data-ttu-id="bb4a7-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="bb4a7-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="bb4a7-118">Tipo de ação de permissão Android.</span><span class="sxs-lookup"><span data-stu-id="bb4a7-118">Type of Android permission action.</span></span> <span data-ttu-id="bb4a7-119">Os valores possíveis são: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="bb4a7-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb4a7-120">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="bb4a7-120">Relationships</span></span>
<span data-ttu-id="bb4a7-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb4a7-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bb4a7-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb4a7-122">JSON Representation</span></span>
<span data-ttu-id="bb4a7-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb4a7-123">Here is a JSON representation of the resource.</span></span>
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





