---
title: tipo de recurso de iosBookmark
description: indicador de URL iOS
ms.openlocfilehash: e2349e0d280c9798a03363ab90d378ff206c57bf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035417"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="f5ad5-103">tipo de recurso de iosBookmark</span><span class="sxs-lookup"><span data-stu-id="f5ad5-103">iosBookmark resource type</span></span>

> <span data-ttu-id="f5ad5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f5ad5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5ad5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f5ad5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5ad5-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f5ad5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5ad5-107">indicador de URL iOS</span><span class="sxs-lookup"><span data-stu-id="f5ad5-107">iOS URL bookmark</span></span>
## <a name="properties"></a><span data-ttu-id="f5ad5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5ad5-108">Properties</span></span>
|<span data-ttu-id="f5ad5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5ad5-109">Property</span></span>|<span data-ttu-id="f5ad5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5ad5-110">Type</span></span>|<span data-ttu-id="f5ad5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5ad5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5ad5-112">url</span><span class="sxs-lookup"><span data-stu-id="f5ad5-112">url</span></span>|<span data-ttu-id="f5ad5-113">String</span><span class="sxs-lookup"><span data-stu-id="f5ad5-113">String</span></span>|<span data-ttu-id="f5ad5-114">URL de permissão para acessar</span><span class="sxs-lookup"><span data-stu-id="f5ad5-114">URL allowed to access</span></span>|
|<span data-ttu-id="f5ad5-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="f5ad5-115">bookmarkFolder</span></span>|<span data-ttu-id="f5ad5-116">String</span><span class="sxs-lookup"><span data-stu-id="f5ad5-116">String</span></span>|<span data-ttu-id="f5ad5-117">A pasta em que o indicador deve ser adicionado no Safari</span><span class="sxs-lookup"><span data-stu-id="f5ad5-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="f5ad5-118">displayName</span><span class="sxs-lookup"><span data-stu-id="f5ad5-118">displayName</span></span>|<span data-ttu-id="f5ad5-119">String</span><span class="sxs-lookup"><span data-stu-id="f5ad5-119">String</span></span>|<span data-ttu-id="f5ad5-120">O nome de exibição do indicador</span><span class="sxs-lookup"><span data-stu-id="f5ad5-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5ad5-121">Relações</span><span class="sxs-lookup"><span data-stu-id="f5ad5-121">Relationships</span></span>
<span data-ttu-id="f5ad5-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5ad5-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f5ad5-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5ad5-123">JSON Representation</span></span>
<span data-ttu-id="f5ad5-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5ad5-124">Here is a JSON representation of the resource.</span></span>
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





