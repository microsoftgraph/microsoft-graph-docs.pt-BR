---
title: Tipo de recurso iosHomeScreenPage
description: Uma página que contém aplicativos e pastas na tela inicial
ms.openlocfilehash: 4f89d32d68b1caef782fa9a023145ad8ea896155
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034288"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="17fec-103">Tipo de recurso iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="17fec-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="17fec-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="17fec-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17fec-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="17fec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17fec-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="17fec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17fec-107">Uma página que contém aplicativos e pastas na tela inicial</span><span class="sxs-lookup"><span data-stu-id="17fec-107">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="17fec-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17fec-108">Properties</span></span>
|<span data-ttu-id="17fec-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17fec-109">Property</span></span>|<span data-ttu-id="17fec-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="17fec-110">Type</span></span>|<span data-ttu-id="17fec-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="17fec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17fec-112">displayName</span><span class="sxs-lookup"><span data-stu-id="17fec-112">displayName</span></span>|<span data-ttu-id="17fec-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17fec-113">String</span></span>|<span data-ttu-id="17fec-114">Nome da página</span><span class="sxs-lookup"><span data-stu-id="17fec-114">Name of the page</span></span>|
|<span data-ttu-id="17fec-115">ícones</span><span class="sxs-lookup"><span data-stu-id="17fec-115">icons</span></span>|<span data-ttu-id="17fec-116">Conjunto [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="17fec-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="17fec-117">Uma lista dos aplicativos e pastas exibidos em uma página.</span><span class="sxs-lookup"><span data-stu-id="17fec-117">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="17fec-118">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="17fec-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17fec-119">Relações</span><span class="sxs-lookup"><span data-stu-id="17fec-119">Relationships</span></span>
<span data-ttu-id="17fec-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="17fec-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="17fec-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17fec-121">JSON Representation</span></span>
<span data-ttu-id="17fec-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="17fec-122">Here is a JSON representation of the resource.</span></span>
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





