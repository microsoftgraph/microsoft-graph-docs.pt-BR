---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bd251fa942d526b01abca4191f041eb5a76745e5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952262"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="ccc2b-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="ccc2b-103">auditProperty resource type</span></span>

> <span data-ttu-id="ccc2b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ccc2b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ccc2b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ccc2b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ccc2b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ccc2b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ccc2b-107">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="ccc2b-107">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="ccc2b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ccc2b-108">Properties</span></span>
|<span data-ttu-id="ccc2b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccc2b-109">Property</span></span>|<span data-ttu-id="ccc2b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccc2b-110">Type</span></span>|<span data-ttu-id="ccc2b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccc2b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccc2b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ccc2b-112">displayName</span></span>|<span data-ttu-id="ccc2b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ccc2b-113">String</span></span>|<span data-ttu-id="ccc2b-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="ccc2b-114">Display name.</span></span>|
|<span data-ttu-id="ccc2b-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="ccc2b-115">oldValue</span></span>|<span data-ttu-id="ccc2b-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ccc2b-116">String</span></span>|<span data-ttu-id="ccc2b-117">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="ccc2b-117">Old value.</span></span>|
|<span data-ttu-id="ccc2b-118">newValue</span><span class="sxs-lookup"><span data-stu-id="ccc2b-118">newValue</span></span>|<span data-ttu-id="ccc2b-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ccc2b-119">String</span></span>|<span data-ttu-id="ccc2b-120">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="ccc2b-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccc2b-121">Relações</span><span class="sxs-lookup"><span data-stu-id="ccc2b-121">Relationships</span></span>
<span data-ttu-id="ccc2b-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ccc2b-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ccc2b-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ccc2b-123">JSON Representation</span></span>
<span data-ttu-id="ccc2b-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ccc2b-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```





