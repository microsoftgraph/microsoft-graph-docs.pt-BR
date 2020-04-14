---
title: Tipo de recurso report
description: Descreve o recurso de relatório da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1e521979060d2892d8a4e135ca52a94fb195d527
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466067"
---
# <a name="report-resource-type"></a><span data-ttu-id="093ff-103">Tipo de recurso report</span><span class="sxs-lookup"><span data-stu-id="093ff-103">report resource type</span></span>

<span data-ttu-id="093ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="093ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="093ff-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="093ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="093ff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="093ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="093ff-107">Retorna o conteúdo apropriado para o contexto, incluindo:</span><span class="sxs-lookup"><span data-stu-id="093ff-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="093ff-108">Relatórios de histórico de perfil de configuração de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="093ff-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="093ff-109">Relatórios de falha de registro.</span><span class="sxs-lookup"><span data-stu-id="093ff-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="093ff-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="093ff-110">Properties</span></span>
|<span data-ttu-id="093ff-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="093ff-111">Property</span></span>|<span data-ttu-id="093ff-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="093ff-112">Type</span></span>|<span data-ttu-id="093ff-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="093ff-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="093ff-114">conteúdo</span><span class="sxs-lookup"><span data-stu-id="093ff-114">content</span></span>|<span data-ttu-id="093ff-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="093ff-115">Stream</span></span>|<span data-ttu-id="093ff-116">Conteúdo de relatórios; os detalhes variam por tipo de relatório.</span><span class="sxs-lookup"><span data-stu-id="093ff-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="093ff-117">Relações</span><span class="sxs-lookup"><span data-stu-id="093ff-117">Relationships</span></span>
<span data-ttu-id="093ff-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="093ff-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="093ff-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="093ff-119">JSON Representation</span></span>
<span data-ttu-id="093ff-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="093ff-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.report"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```



