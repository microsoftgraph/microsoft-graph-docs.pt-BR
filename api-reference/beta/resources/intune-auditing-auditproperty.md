---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3425c59ae4f30b30b04bd22f74cb1b27ad99191f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416640"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="aefd0-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="aefd0-103">auditProperty resource type</span></span>

> <span data-ttu-id="aefd0-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="aefd0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aefd0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="aefd0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aefd0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="aefd0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aefd0-107">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="aefd0-107">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="aefd0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aefd0-108">Properties</span></span>
|<span data-ttu-id="aefd0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aefd0-109">Property</span></span>|<span data-ttu-id="aefd0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="aefd0-110">Type</span></span>|<span data-ttu-id="aefd0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="aefd0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aefd0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="aefd0-112">displayName</span></span>|<span data-ttu-id="aefd0-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aefd0-113">String</span></span>|<span data-ttu-id="aefd0-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="aefd0-114">Display name.</span></span>|
|<span data-ttu-id="aefd0-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="aefd0-115">oldValue</span></span>|<span data-ttu-id="aefd0-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aefd0-116">String</span></span>|<span data-ttu-id="aefd0-117">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="aefd0-117">Old value.</span></span>|
|<span data-ttu-id="aefd0-118">newValue</span><span class="sxs-lookup"><span data-stu-id="aefd0-118">newValue</span></span>|<span data-ttu-id="aefd0-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aefd0-119">String</span></span>|<span data-ttu-id="aefd0-120">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="aefd0-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aefd0-121">Relações</span><span class="sxs-lookup"><span data-stu-id="aefd0-121">Relationships</span></span>
<span data-ttu-id="aefd0-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aefd0-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aefd0-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aefd0-123">JSON Representation</span></span>
<span data-ttu-id="aefd0-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aefd0-124">Here is a JSON representation of the resource.</span></span>
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




