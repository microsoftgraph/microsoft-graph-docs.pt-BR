---
title: Tipo de recurso report
description: Descreve o recurso de relatório da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: f94be1bcc5dfde092c6360bbdddd96d604d30a55
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939669"
---
# <a name="report-resource-type"></a><span data-ttu-id="07cd6-103">Tipo de recurso report</span><span class="sxs-lookup"><span data-stu-id="07cd6-103">report resource type</span></span>

> <span data-ttu-id="07cd6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07cd6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07cd6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07cd6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07cd6-106">Retorna o conteúdo apropriado para o contexto, incluindo:</span><span class="sxs-lookup"><span data-stu-id="07cd6-106">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="07cd6-107">Relatórios de histórico de perfil de configuração de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="07cd6-107">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="07cd6-108">Relatórios de falha de registro.</span><span class="sxs-lookup"><span data-stu-id="07cd6-108">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="07cd6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07cd6-109">Properties</span></span>
|<span data-ttu-id="07cd6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07cd6-110">Property</span></span>|<span data-ttu-id="07cd6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="07cd6-111">Type</span></span>|<span data-ttu-id="07cd6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="07cd6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07cd6-113">conteúdo</span><span class="sxs-lookup"><span data-stu-id="07cd6-113">content</span></span>|<span data-ttu-id="07cd6-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="07cd6-114">Stream</span></span>|<span data-ttu-id="07cd6-115">Conteúdo de relatórios; os detalhes variam por tipo de relatório.</span><span class="sxs-lookup"><span data-stu-id="07cd6-115">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07cd6-116">Relações</span><span class="sxs-lookup"><span data-stu-id="07cd6-116">Relationships</span></span>
<span data-ttu-id="07cd6-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="07cd6-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07cd6-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07cd6-118">JSON Representation</span></span>
<span data-ttu-id="07cd6-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07cd6-119">Here is a JSON representation of the resource.</span></span>
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



