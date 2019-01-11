---
title: tipo de recurso de extendedKeyUsage
description: Definição de uso estendido de chave personalizada
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f1fd159a9b9fdb621a1e52bd080c005c8b93129c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840975"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="de24c-103">tipo de recurso de extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="de24c-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="de24c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="de24c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de24c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="de24c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de24c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="de24c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de24c-107">Definição de uso estendido de chave personalizada</span><span class="sxs-lookup"><span data-stu-id="de24c-107">Custom Extended Key Usage definition</span></span>
## <a name="properties"></a><span data-ttu-id="de24c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de24c-108">Properties</span></span>
|<span data-ttu-id="de24c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de24c-109">Property</span></span>|<span data-ttu-id="de24c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="de24c-110">Type</span></span>|<span data-ttu-id="de24c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="de24c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de24c-112">name</span><span class="sxs-lookup"><span data-stu-id="de24c-112">name</span></span>|<span data-ttu-id="de24c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de24c-113">String</span></span>|<span data-ttu-id="de24c-114">Nome do uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="de24c-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="de24c-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="de24c-115">objectIdentifier</span></span>|<span data-ttu-id="de24c-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de24c-116">String</span></span>|<span data-ttu-id="de24c-117">Identificador de objeto de uso da chave de estendido</span><span class="sxs-lookup"><span data-stu-id="de24c-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="de24c-118">Relações</span><span class="sxs-lookup"><span data-stu-id="de24c-118">Relationships</span></span>
<span data-ttu-id="de24c-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de24c-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="de24c-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de24c-120">JSON Representation</span></span>
<span data-ttu-id="de24c-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de24c-121">Here is a JSON representation of the resource.</span></span>
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





