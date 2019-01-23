---
title: Tipo de recurso report
description: Descreve o recurso de relatório da API Microsoft Graph para Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 098c20b2460324c4975533902e1b71fde1af41c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407470"
---
# <a name="report-resource-type"></a><span data-ttu-id="f68b0-103">Tipo de recurso report</span><span class="sxs-lookup"><span data-stu-id="f68b0-103">report resource type</span></span>

> <span data-ttu-id="f68b0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f68b0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f68b0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f68b0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f68b0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f68b0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f68b0-107">Retorna o conteúdo apropriada para o contexto, incluindo:</span><span class="sxs-lookup"><span data-stu-id="f68b0-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="f68b0-108">Relatórios de histórico de perfil de configuração de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f68b0-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="f68b0-109">Relatórios de falha de inscrição.</span><span class="sxs-lookup"><span data-stu-id="f68b0-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="f68b0-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f68b0-110">Properties</span></span>
|<span data-ttu-id="f68b0-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f68b0-111">Property</span></span>|<span data-ttu-id="f68b0-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="f68b0-112">Type</span></span>|<span data-ttu-id="f68b0-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f68b0-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f68b0-114">content</span><span class="sxs-lookup"><span data-stu-id="f68b0-114">content</span></span>|<span data-ttu-id="f68b0-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="f68b0-115">Stream</span></span>|<span data-ttu-id="f68b0-116">Relatório de conteúdo; detalhes variam de acordo com o tipo de relatório.</span><span class="sxs-lookup"><span data-stu-id="f68b0-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f68b0-117">Relações</span><span class="sxs-lookup"><span data-stu-id="f68b0-117">Relationships</span></span>
<span data-ttu-id="f68b0-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f68b0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f68b0-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f68b0-119">JSON Representation</span></span>
<span data-ttu-id="f68b0-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f68b0-120">Here is a JSON representation of the resource.</span></span>
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



