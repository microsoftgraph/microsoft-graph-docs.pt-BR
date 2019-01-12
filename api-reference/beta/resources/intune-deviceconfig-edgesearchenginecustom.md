---
title: Tipo de recurso edgeSearchEngineCustom
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8171c293610efc790eadc0619c99fe604d6c933b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932886"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="fe8c1-103">Tipo de recurso edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="fe8c1-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="fe8c1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fe8c1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe8c1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fe8c1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe8c1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fe8c1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe8c1-107">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="fe8c1-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="fe8c1-108">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="fe8c1-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fe8c1-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe8c1-109">Properties</span></span>
|<span data-ttu-id="fe8c1-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe8c1-110">Property</span></span>|<span data-ttu-id="fe8c1-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe8c1-111">Type</span></span>|<span data-ttu-id="fe8c1-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe8c1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe8c1-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="fe8c1-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="fe8c1-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe8c1-114">String</span></span>|<span data-ttu-id="fe8c1-115">Aponta para um link https que contém o arquivo xml de OpenSearch que contém no mínimo o nome curto e a URL do mecanismo de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="fe8c1-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe8c1-116">Relações</span><span class="sxs-lookup"><span data-stu-id="fe8c1-116">Relationships</span></span>
<span data-ttu-id="fe8c1-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fe8c1-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fe8c1-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe8c1-118">JSON Representation</span></span>
<span data-ttu-id="fe8c1-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe8c1-119">Here is a JSON representation of the resource.</span></span>
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





