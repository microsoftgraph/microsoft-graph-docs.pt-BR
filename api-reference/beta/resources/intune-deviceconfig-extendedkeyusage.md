---
title: tipo de recurso de extendedKeyUsage
description: Definição de uso estendido de chave personalizada
ms.openlocfilehash: bbf869dd32c384a12aa8e80e8a3b5984e699de48
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033194"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="5cb8a-103">tipo de recurso de extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="5cb8a-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="5cb8a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5cb8a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5cb8a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5cb8a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5cb8a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5cb8a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5cb8a-107">Definição de uso estendido de chave personalizada</span><span class="sxs-lookup"><span data-stu-id="5cb8a-107">Custom Extended Key Usage definition</span></span>
## <a name="properties"></a><span data-ttu-id="5cb8a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5cb8a-108">Properties</span></span>
|<span data-ttu-id="5cb8a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5cb8a-109">Property</span></span>|<span data-ttu-id="5cb8a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cb8a-110">Type</span></span>|<span data-ttu-id="5cb8a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cb8a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cb8a-112">name</span><span class="sxs-lookup"><span data-stu-id="5cb8a-112">name</span></span>|<span data-ttu-id="5cb8a-113">String</span><span class="sxs-lookup"><span data-stu-id="5cb8a-113">String</span></span>|<span data-ttu-id="5cb8a-114">Nome do uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="5cb8a-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="5cb8a-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="5cb8a-115">objectIdentifier</span></span>|<span data-ttu-id="5cb8a-116">String</span><span class="sxs-lookup"><span data-stu-id="5cb8a-116">String</span></span>|<span data-ttu-id="5cb8a-117">Identificador de objeto de uso da chave de estendido</span><span class="sxs-lookup"><span data-stu-id="5cb8a-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cb8a-118">Relações</span><span class="sxs-lookup"><span data-stu-id="5cb8a-118">Relationships</span></span>
<span data-ttu-id="5cb8a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5cb8a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5cb8a-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5cb8a-120">JSON Representation</span></span>
<span data-ttu-id="5cb8a-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5cb8a-121">Here is a JSON representation of the resource.</span></span>
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





