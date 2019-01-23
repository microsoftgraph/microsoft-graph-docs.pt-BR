---
title: tipo de recurso de iosBookmark
description: indicador de URL iOS
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e95f3bfd40bdf5ca5782aa9233a020623d32d6a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395906"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="f6484-103">tipo de recurso de iosBookmark</span><span class="sxs-lookup"><span data-stu-id="f6484-103">iosBookmark resource type</span></span>

> <span data-ttu-id="f6484-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f6484-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f6484-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f6484-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6484-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f6484-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6484-107">indicador de URL iOS</span><span class="sxs-lookup"><span data-stu-id="f6484-107">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="f6484-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6484-108">Properties</span></span>
|<span data-ttu-id="f6484-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6484-109">Property</span></span>|<span data-ttu-id="f6484-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6484-110">Type</span></span>|<span data-ttu-id="f6484-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6484-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6484-112">url</span><span class="sxs-lookup"><span data-stu-id="f6484-112">url</span></span>|<span data-ttu-id="f6484-113">String</span><span class="sxs-lookup"><span data-stu-id="f6484-113">String</span></span>|<span data-ttu-id="f6484-114">URL de permissão para acessar</span><span class="sxs-lookup"><span data-stu-id="f6484-114">URL allowed to access</span></span>|
|<span data-ttu-id="f6484-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="f6484-115">bookmarkFolder</span></span>|<span data-ttu-id="f6484-116">String</span><span class="sxs-lookup"><span data-stu-id="f6484-116">String</span></span>|<span data-ttu-id="f6484-117">A pasta em que o indicador deve ser adicionado no Safari</span><span class="sxs-lookup"><span data-stu-id="f6484-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="f6484-118">displayName</span><span class="sxs-lookup"><span data-stu-id="f6484-118">displayName</span></span>|<span data-ttu-id="f6484-119">String</span><span class="sxs-lookup"><span data-stu-id="f6484-119">String</span></span>|<span data-ttu-id="f6484-120">O nome de exibição do indicador</span><span class="sxs-lookup"><span data-stu-id="f6484-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6484-121">Relações</span><span class="sxs-lookup"><span data-stu-id="f6484-121">Relationships</span></span>
<span data-ttu-id="f6484-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f6484-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6484-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6484-123">JSON Representation</span></span>
<span data-ttu-id="f6484-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f6484-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosBookmark"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosBookmark",
  "url": "String",
  "bookmarkFolder": "String",
  "displayName": "String"
}
```




