---
title: Tipo de recurso resourceAction
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: c373cc15b1dfce1ca3cede9fa1c7a642da48f5bf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319156"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="379f7-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="379f7-103">resourceAction resource type</span></span>

> <span data-ttu-id="379f7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="379f7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="379f7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="379f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="379f7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="379f7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="379f7-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="379f7-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="379f7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="379f7-108">Properties</span></span>
|<span data-ttu-id="379f7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="379f7-109">Property</span></span>|<span data-ttu-id="379f7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="379f7-110">Type</span></span>|<span data-ttu-id="379f7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="379f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="379f7-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="379f7-112">allowedResourceActions</span></span>|<span data-ttu-id="379f7-113">String collection</span><span class="sxs-lookup"><span data-stu-id="379f7-113">String collection</span></span>|<span data-ttu-id="379f7-114">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="379f7-114">Allowed Actions</span></span>|
|<span data-ttu-id="379f7-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="379f7-115">notAllowedResourceActions</span></span>|<span data-ttu-id="379f7-116">String collection</span><span class="sxs-lookup"><span data-stu-id="379f7-116">String collection</span></span>|<span data-ttu-id="379f7-117">Ações não permitidas</span><span class="sxs-lookup"><span data-stu-id="379f7-117">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="379f7-118">Relações</span><span class="sxs-lookup"><span data-stu-id="379f7-118">Relationships</span></span>
<span data-ttu-id="379f7-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="379f7-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="379f7-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="379f7-120">JSON Representation</span></span>
<span data-ttu-id="379f7-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="379f7-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```





