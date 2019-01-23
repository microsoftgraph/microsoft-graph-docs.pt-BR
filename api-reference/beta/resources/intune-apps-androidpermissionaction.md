---
title: tipo de recurso de androidPermissionAction
description: Mapeamento entre uma permissão de app Android e a ação Android deve ser adotada quando essa permissão é solicitada.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62355c3427083df09963e316f3b6b3c104a8662f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425628"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="af71a-103">tipo de recurso de androidPermissionAction</span><span class="sxs-lookup"><span data-stu-id="af71a-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="af71a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="af71a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="af71a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="af71a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af71a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="af71a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af71a-107">Mapeamento entre uma permissão de app Android e a ação Android deve ser adotada quando essa permissão é solicitada.</span><span class="sxs-lookup"><span data-stu-id="af71a-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="af71a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af71a-108">Properties</span></span>
|<span data-ttu-id="af71a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af71a-109">Property</span></span>|<span data-ttu-id="af71a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="af71a-110">Type</span></span>|<span data-ttu-id="af71a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="af71a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af71a-112">permissão</span><span class="sxs-lookup"><span data-stu-id="af71a-112">permission</span></span>|<span data-ttu-id="af71a-113">String</span><span class="sxs-lookup"><span data-stu-id="af71a-113">String</span></span>|<span data-ttu-id="af71a-114">String de permissão Android, definido na documentação oficial Android.</span><span class="sxs-lookup"><span data-stu-id="af71a-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="af71a-115">Exemplo 'android.permission.READ_CONTACTS'.</span><span class="sxs-lookup"><span data-stu-id="af71a-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="af71a-116">action</span><span class="sxs-lookup"><span data-stu-id="af71a-116">action</span></span>|[<span data-ttu-id="af71a-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="af71a-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="af71a-118">Tipo de ação de permissão Android.</span><span class="sxs-lookup"><span data-stu-id="af71a-118">Type of Android permission action.</span></span> <span data-ttu-id="af71a-119">Os valores possíveis são: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="af71a-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af71a-120">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="af71a-120">Relationships</span></span>
<span data-ttu-id="af71a-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af71a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af71a-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af71a-122">JSON Representation</span></span>
<span data-ttu-id="af71a-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="af71a-123">Here is a JSON representation of the resource.</span></span>
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




