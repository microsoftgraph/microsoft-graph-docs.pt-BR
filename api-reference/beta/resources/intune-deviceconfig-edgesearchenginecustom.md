---
title: Tipo de recurso edgeSearchEngineCustom
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f960c68e0ecce4cebdbd4727c77eae971cb5ce70
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530042"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="8e371-103">Tipo de recurso edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="8e371-103">edgeSearchEngineCustom resource type</span></span>

<span data-ttu-id="8e371-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8e371-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e371-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e371-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e371-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e371-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e371-107">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="8e371-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="8e371-108">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="8e371-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8e371-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e371-109">Properties</span></span>
|<span data-ttu-id="8e371-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e371-110">Property</span></span>|<span data-ttu-id="8e371-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e371-111">Type</span></span>|<span data-ttu-id="8e371-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e371-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e371-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="8e371-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="8e371-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e371-114">String</span></span>|<span data-ttu-id="8e371-115">Aponta para um link https que contém o arquivo xml de OpenSearch que contém no mínimo o nome curto e a URL do mecanismo de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8e371-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e371-116">Relações</span><span class="sxs-lookup"><span data-stu-id="8e371-116">Relationships</span></span>
<span data-ttu-id="8e371-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e371-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e371-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e371-118">JSON Representation</span></span>
<span data-ttu-id="8e371-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e371-119">Here is a JSON representation of the resource.</span></span>
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



