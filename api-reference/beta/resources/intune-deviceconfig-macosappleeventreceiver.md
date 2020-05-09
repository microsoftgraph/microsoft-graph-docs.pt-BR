---
title: tipo de recurso macOSAppleEventReceiver
description: Representa um processo que pode receber uma notificação de evento Apple.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 16064b1f7311f8ab384d7905a6f4cfa2f09ccc09
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177349"
---
# <a name="macosappleeventreceiver-resource-type"></a><span data-ttu-id="cf182-103">tipo de recurso macOSAppleEventReceiver</span><span class="sxs-lookup"><span data-stu-id="cf182-103">macOSAppleEventReceiver resource type</span></span>

<span data-ttu-id="cf182-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf182-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf182-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf182-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf182-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf182-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf182-107">Representa um processo que pode receber uma notificação de evento Apple.</span><span class="sxs-lookup"><span data-stu-id="cf182-107">Represents a process that can receive an Apple Event notification.</span></span>

## <a name="properties"></a><span data-ttu-id="cf182-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf182-108">Properties</span></span>
|<span data-ttu-id="cf182-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf182-109">Property</span></span>|<span data-ttu-id="cf182-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf182-110">Type</span></span>|<span data-ttu-id="cf182-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf182-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf182-112">codeRequirement</span><span class="sxs-lookup"><span data-stu-id="cf182-112">codeRequirement</span></span>|<span data-ttu-id="cf182-113">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cf182-113">String</span></span>|<span data-ttu-id="cf182-114">Requisito de código para o aplicativo ou o binário que recebe o evento Apple.</span><span class="sxs-lookup"><span data-stu-id="cf182-114">Code requirement for the app or binary that receives the Apple Event.</span></span>|
|<span data-ttu-id="cf182-115">identificador</span><span class="sxs-lookup"><span data-stu-id="cf182-115">identifier</span></span>|<span data-ttu-id="cf182-116">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cf182-116">String</span></span>|<span data-ttu-id="cf182-117">ID de pacote do aplicativo ou caminho de arquivo do processo ou executável que recebe o evento Apple.</span><span class="sxs-lookup"><span data-stu-id="cf182-117">Bundle ID of the app or file path of the process or executable that receives the Apple Event.</span></span>|
|<span data-ttu-id="cf182-118">identifierType</span><span class="sxs-lookup"><span data-stu-id="cf182-118">identifierType</span></span>|[<span data-ttu-id="cf182-119">macOSProcessIdentifierType</span><span class="sxs-lookup"><span data-stu-id="cf182-119">macOSProcessIdentifierType</span></span>](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|<span data-ttu-id="cf182-120">Use ID de pacote para um aplicativo ou caminho para um processo ou executável que receba o evento Apple.</span><span class="sxs-lookup"><span data-stu-id="cf182-120">Use bundle ID for an app or path for a process or executable that receives the Apple Event.</span></span> <span data-ttu-id="cf182-121">Os valores possíveis são: `bundleID` e `path`.</span><span class="sxs-lookup"><span data-stu-id="cf182-121">Possible values are: `bundleID`, `path`.</span></span>|
|<span data-ttu-id="cf182-122">autorizado</span><span class="sxs-lookup"><span data-stu-id="cf182-122">allowed</span></span>|<span data-ttu-id="cf182-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf182-123">Boolean</span></span>|<span data-ttu-id="cf182-124">Permitir ou impedir que este aplicativo receba eventos Apple.</span><span class="sxs-lookup"><span data-stu-id="cf182-124">Allow or block this app from receiving Apple events.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf182-125">Relações</span><span class="sxs-lookup"><span data-stu-id="cf182-125">Relationships</span></span>
<span data-ttu-id="cf182-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cf182-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf182-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf182-127">JSON Representation</span></span>
<span data-ttu-id="cf182-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf182-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAppleEventReceiver"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAppleEventReceiver",
  "codeRequirement": "String",
  "identifier": "String",
  "identifierType": "String",
  "allowed": true
}
```



