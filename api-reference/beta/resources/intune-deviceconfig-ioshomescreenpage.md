---
title: Tipo de recurso iosHomeScreenPage
description: Uma página que contém aplicativos e pastas na tela inicial
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a59c910f37a82e04a7ccd5050a0a03999ac567b7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961033"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="4242d-103">Tipo de recurso iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="4242d-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="4242d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4242d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4242d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4242d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4242d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4242d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4242d-107">Uma página que contém aplicativos e pastas na tela inicial</span><span class="sxs-lookup"><span data-stu-id="4242d-107">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="4242d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4242d-108">Properties</span></span>
|<span data-ttu-id="4242d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4242d-109">Property</span></span>|<span data-ttu-id="4242d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4242d-110">Type</span></span>|<span data-ttu-id="4242d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4242d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4242d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4242d-112">displayName</span></span>|<span data-ttu-id="4242d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4242d-113">String</span></span>|<span data-ttu-id="4242d-114">Nome da página</span><span class="sxs-lookup"><span data-stu-id="4242d-114">Name of the page</span></span>|
|<span data-ttu-id="4242d-115">ícones</span><span class="sxs-lookup"><span data-stu-id="4242d-115">icons</span></span>|<span data-ttu-id="4242d-116">Conjunto [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="4242d-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="4242d-117">Uma lista dos aplicativos e pastas exibidos em uma página.</span><span class="sxs-lookup"><span data-stu-id="4242d-117">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="4242d-118">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="4242d-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4242d-119">Relações</span><span class="sxs-lookup"><span data-stu-id="4242d-119">Relationships</span></span>
<span data-ttu-id="4242d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4242d-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4242d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4242d-121">JSON Representation</span></span>
<span data-ttu-id="4242d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4242d-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "String",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "String",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "String",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ]
}
```





