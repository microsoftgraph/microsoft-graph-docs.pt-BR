---
title: Tipo de recurso iosHomeScreenPage
description: Uma página que contém aplicativos e pastas na tela inicial
ms.openlocfilehash: 4ef336bc104a203739904b67e301b489627e7ff1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005018"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="66113-103">Tipo de recurso iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="66113-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="66113-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="66113-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66113-105">Uma página que contém aplicativos e pastas na tela inicial</span><span class="sxs-lookup"><span data-stu-id="66113-105">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="66113-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66113-106">Properties</span></span>
|<span data-ttu-id="66113-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66113-107">Property</span></span>|<span data-ttu-id="66113-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="66113-108">Type</span></span>|<span data-ttu-id="66113-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="66113-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66113-110">displayName</span><span class="sxs-lookup"><span data-stu-id="66113-110">displayName</span></span>|<span data-ttu-id="66113-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66113-111">String</span></span>|<span data-ttu-id="66113-112">Nome da página</span><span class="sxs-lookup"><span data-stu-id="66113-112">Name of the page</span></span>|
|<span data-ttu-id="66113-113">ícones</span><span class="sxs-lookup"><span data-stu-id="66113-113">icons</span></span>|<span data-ttu-id="66113-114">Conjunto [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="66113-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="66113-115">Uma lista dos aplicativos e pastas exibidos em uma página.</span><span class="sxs-lookup"><span data-stu-id="66113-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="66113-116">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="66113-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66113-117">Relações</span><span class="sxs-lookup"><span data-stu-id="66113-117">Relationships</span></span>
<span data-ttu-id="66113-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66113-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="66113-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66113-119">JSON Representation</span></span>
<span data-ttu-id="66113-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66113-120">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.iosHomeScreenItem",
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



