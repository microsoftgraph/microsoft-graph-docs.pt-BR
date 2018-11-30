---
title: Tipo de recurso report
description: 'Retorna o conteúdo apropriada para o contexto, incluindo:'
ms.openlocfilehash: b05e5db2b948455f14746cf23a07b3fd788ccad9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038550"
---
# <a name="report-resource-type"></a><span data-ttu-id="2d62d-103">Tipo de recurso report</span><span class="sxs-lookup"><span data-stu-id="2d62d-103">report resource type</span></span>

> <span data-ttu-id="2d62d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2d62d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d62d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2d62d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2d62d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2d62d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d62d-107">Retorna o conteúdo apropriada para o contexto, incluindo:</span><span class="sxs-lookup"><span data-stu-id="2d62d-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="2d62d-108">Relatórios de histórico de perfil de configuração de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2d62d-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="2d62d-109">Relatórios de falha de inscrição.</span><span class="sxs-lookup"><span data-stu-id="2d62d-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="2d62d-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d62d-110">Properties</span></span>
|<span data-ttu-id="2d62d-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d62d-111">Property</span></span>|<span data-ttu-id="2d62d-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d62d-112">Type</span></span>|<span data-ttu-id="2d62d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d62d-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d62d-114">content</span><span class="sxs-lookup"><span data-stu-id="2d62d-114">content</span></span>|<span data-ttu-id="2d62d-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="2d62d-115">Stream</span></span>|<span data-ttu-id="2d62d-116">Relatório de conteúdo; detalhes variam de acordo com o tipo de relatório.</span><span class="sxs-lookup"><span data-stu-id="2d62d-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d62d-117">Relações</span><span class="sxs-lookup"><span data-stu-id="2d62d-117">Relationships</span></span>
<span data-ttu-id="2d62d-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2d62d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d62d-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d62d-119">JSON Representation</span></span>
<span data-ttu-id="2d62d-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d62d-120">Here is a JSON representation of the resource.</span></span>
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



