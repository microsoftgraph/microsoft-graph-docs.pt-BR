---
title: tipo de recurso de extendedKeyUsage
description: Definição de uso estendido de chave personalizada
author: tfitzmac
ms.openlocfilehash: 2b6155a0fbb234cb0b2081a8a4a226a8d218dbc2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337286"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="dfa6b-103">tipo de recurso de extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="dfa6b-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="dfa6b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dfa6b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfa6b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dfa6b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dfa6b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dfa6b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dfa6b-107">Definição de uso estendido de chave personalizada</span><span class="sxs-lookup"><span data-stu-id="dfa6b-107">Custom Extended Key Usage definition</span></span>
## <a name="properties"></a><span data-ttu-id="dfa6b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dfa6b-108">Properties</span></span>
|<span data-ttu-id="dfa6b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dfa6b-109">Property</span></span>|<span data-ttu-id="dfa6b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfa6b-110">Type</span></span>|<span data-ttu-id="dfa6b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfa6b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfa6b-112">name</span><span class="sxs-lookup"><span data-stu-id="dfa6b-112">name</span></span>|<span data-ttu-id="dfa6b-113">String</span><span class="sxs-lookup"><span data-stu-id="dfa6b-113">String</span></span>|<span data-ttu-id="dfa6b-114">Nome do uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="dfa6b-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="dfa6b-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="dfa6b-115">objectIdentifier</span></span>|<span data-ttu-id="dfa6b-116">String</span><span class="sxs-lookup"><span data-stu-id="dfa6b-116">String</span></span>|<span data-ttu-id="dfa6b-117">Identificador de objeto de uso da chave de estendido</span><span class="sxs-lookup"><span data-stu-id="dfa6b-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfa6b-118">Relações</span><span class="sxs-lookup"><span data-stu-id="dfa6b-118">Relationships</span></span>
<span data-ttu-id="dfa6b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dfa6b-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dfa6b-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dfa6b-120">JSON Representation</span></span>
<span data-ttu-id="dfa6b-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dfa6b-121">Here is a JSON representation of the resource.</span></span>
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





