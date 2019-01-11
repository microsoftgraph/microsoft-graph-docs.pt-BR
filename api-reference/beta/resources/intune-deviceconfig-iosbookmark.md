---
title: tipo de recurso de iosBookmark
description: indicador de URL iOS
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 37cdcc1b886914b4b42e0a97e8947a565c75f5b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840996"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="81fb6-103">tipo de recurso de iosBookmark</span><span class="sxs-lookup"><span data-stu-id="81fb6-103">iosBookmark resource type</span></span>

> <span data-ttu-id="81fb6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="81fb6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81fb6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="81fb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81fb6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="81fb6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81fb6-107">indicador de URL iOS</span><span class="sxs-lookup"><span data-stu-id="81fb6-107">iOS URL bookmark</span></span>
## <a name="properties"></a><span data-ttu-id="81fb6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81fb6-108">Properties</span></span>
|<span data-ttu-id="81fb6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81fb6-109">Property</span></span>|<span data-ttu-id="81fb6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="81fb6-110">Type</span></span>|<span data-ttu-id="81fb6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="81fb6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81fb6-112">url</span><span class="sxs-lookup"><span data-stu-id="81fb6-112">url</span></span>|<span data-ttu-id="81fb6-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81fb6-113">String</span></span>|<span data-ttu-id="81fb6-114">URL de permissão para acessar</span><span class="sxs-lookup"><span data-stu-id="81fb6-114">URL allowed to access</span></span>|
|<span data-ttu-id="81fb6-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="81fb6-115">bookmarkFolder</span></span>|<span data-ttu-id="81fb6-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81fb6-116">String</span></span>|<span data-ttu-id="81fb6-117">A pasta em que o indicador deve ser adicionado no Safari</span><span class="sxs-lookup"><span data-stu-id="81fb6-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="81fb6-118">displayName</span><span class="sxs-lookup"><span data-stu-id="81fb6-118">displayName</span></span>|<span data-ttu-id="81fb6-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81fb6-119">String</span></span>|<span data-ttu-id="81fb6-120">O nome de exibição do indicador</span><span class="sxs-lookup"><span data-stu-id="81fb6-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="81fb6-121">Relações</span><span class="sxs-lookup"><span data-stu-id="81fb6-121">Relationships</span></span>
<span data-ttu-id="81fb6-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81fb6-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="81fb6-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81fb6-123">JSON Representation</span></span>
<span data-ttu-id="81fb6-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81fb6-124">Here is a JSON representation of the resource.</span></span>
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





