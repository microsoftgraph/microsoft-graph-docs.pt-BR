---
title: tipo de recurso de extendedKeyUsage
description: Definição de uso estendido de chave personalizada
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bb08bf086ce8386e424ebd6355a4920e87be59a0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928441"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="7f62f-103">tipo de recurso de extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="7f62f-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="7f62f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7f62f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f62f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7f62f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f62f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7f62f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f62f-107">Definição de uso estendido de chave personalizada</span><span class="sxs-lookup"><span data-stu-id="7f62f-107">Custom Extended Key Usage definition</span></span>
## <a name="properties"></a><span data-ttu-id="7f62f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f62f-108">Properties</span></span>
|<span data-ttu-id="7f62f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f62f-109">Property</span></span>|<span data-ttu-id="7f62f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f62f-110">Type</span></span>|<span data-ttu-id="7f62f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f62f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f62f-112">name</span><span class="sxs-lookup"><span data-stu-id="7f62f-112">name</span></span>|<span data-ttu-id="7f62f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f62f-113">String</span></span>|<span data-ttu-id="7f62f-114">Nome do uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="7f62f-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="7f62f-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="7f62f-115">objectIdentifier</span></span>|<span data-ttu-id="7f62f-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f62f-116">String</span></span>|<span data-ttu-id="7f62f-117">Identificador de objeto de uso da chave de estendido</span><span class="sxs-lookup"><span data-stu-id="7f62f-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f62f-118">Relações</span><span class="sxs-lookup"><span data-stu-id="7f62f-118">Relationships</span></span>
<span data-ttu-id="7f62f-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7f62f-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7f62f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f62f-120">JSON Representation</span></span>
<span data-ttu-id="7f62f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f62f-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```





