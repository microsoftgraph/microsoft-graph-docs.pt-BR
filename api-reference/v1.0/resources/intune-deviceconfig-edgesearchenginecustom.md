---
title: Tipo de recurso edgeSearchEngineCustom
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.
author: tfitzmac
ms.openlocfilehash: f648f41bafcbaa37c972500139ecc8d3e70113ca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357971"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="c9931-103">Tipo de recurso edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="c9931-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="c9931-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c9931-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9931-105">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="c9931-105">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="c9931-106">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="c9931-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9931-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9931-107">Properties</span></span>
|<span data-ttu-id="c9931-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9931-108">Property</span></span>|<span data-ttu-id="c9931-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9931-109">Type</span></span>|<span data-ttu-id="c9931-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9931-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9931-111">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="c9931-111">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="c9931-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9931-112">String</span></span>|<span data-ttu-id="c9931-113">Aponta para um link https que contém o arquivo xml de OpenSearch que contém no mínimo o nome curto e a URL do mecanismo de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c9931-113">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9931-114">Relações</span><span class="sxs-lookup"><span data-stu-id="c9931-114">Relationships</span></span>
<span data-ttu-id="c9931-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c9931-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c9931-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9931-116">JSON Representation</span></span>
<span data-ttu-id="c9931-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9931-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```



