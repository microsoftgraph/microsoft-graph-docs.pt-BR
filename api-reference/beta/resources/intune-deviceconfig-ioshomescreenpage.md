---
title: Tipo de recurso iosHomeScreenPage
description: Uma página que contém aplicativos e pastas na tela inicial
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b2b6e4ba9cc70253e929a0f434a292aeafd24bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398545"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="cad48-103">Tipo de recurso iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="cad48-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="cad48-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="cad48-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cad48-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cad48-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cad48-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cad48-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cad48-107">Uma página que contém aplicativos e pastas na tela inicial</span><span class="sxs-lookup"><span data-stu-id="cad48-107">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="cad48-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cad48-108">Properties</span></span>
|<span data-ttu-id="cad48-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cad48-109">Property</span></span>|<span data-ttu-id="cad48-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cad48-110">Type</span></span>|<span data-ttu-id="cad48-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cad48-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cad48-112">displayName</span><span class="sxs-lookup"><span data-stu-id="cad48-112">displayName</span></span>|<span data-ttu-id="cad48-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cad48-113">String</span></span>|<span data-ttu-id="cad48-114">Nome da página</span><span class="sxs-lookup"><span data-stu-id="cad48-114">Name of the page</span></span>|
|<span data-ttu-id="cad48-115">ícones</span><span class="sxs-lookup"><span data-stu-id="cad48-115">icons</span></span>|<span data-ttu-id="cad48-116">Conjunto [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="cad48-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="cad48-117">Uma lista dos aplicativos e pastas exibidos em uma página.</span><span class="sxs-lookup"><span data-stu-id="cad48-117">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="cad48-118">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="cad48-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cad48-119">Relações</span><span class="sxs-lookup"><span data-stu-id="cad48-119">Relationships</span></span>
<span data-ttu-id="cad48-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cad48-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cad48-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cad48-121">JSON Representation</span></span>
<span data-ttu-id="cad48-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cad48-122">Here is a JSON representation of the resource.</span></span>
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




