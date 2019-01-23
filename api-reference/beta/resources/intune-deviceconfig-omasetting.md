---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fdf74ba7e8932ce06bca83d88336239c2abcacf4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411033"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="6a092-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="6a092-103">omaSetting resource type</span></span>

> <span data-ttu-id="6a092-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="6a092-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6a092-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6a092-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a092-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="6a092-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a092-107">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="6a092-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="6a092-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a092-108">Properties</span></span>
|<span data-ttu-id="6a092-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a092-109">Property</span></span>|<span data-ttu-id="6a092-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a092-110">Type</span></span>|<span data-ttu-id="6a092-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a092-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a092-112">displayName</span><span class="sxs-lookup"><span data-stu-id="6a092-112">displayName</span></span>|<span data-ttu-id="6a092-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a092-113">String</span></span>|<span data-ttu-id="6a092-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="6a092-114">Display Name.</span></span>|
|<span data-ttu-id="6a092-115">descrição</span><span class="sxs-lookup"><span data-stu-id="6a092-115">description</span></span>|<span data-ttu-id="6a092-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a092-116">String</span></span>|<span data-ttu-id="6a092-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="6a092-117">Description.</span></span>|
|<span data-ttu-id="6a092-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="6a092-118">omaUri</span></span>|<span data-ttu-id="6a092-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a092-119">String</span></span>|<span data-ttu-id="6a092-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="6a092-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a092-121">Relações</span><span class="sxs-lookup"><span data-stu-id="6a092-121">Relationships</span></span>
<span data-ttu-id="6a092-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a092-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a092-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a092-123">JSON Representation</span></span>
<span data-ttu-id="6a092-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a092-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```




