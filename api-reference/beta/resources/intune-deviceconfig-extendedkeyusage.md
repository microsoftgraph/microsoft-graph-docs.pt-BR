---
title: tipo de recurso de extendedKeyUsage
description: Definição de uso estendido de chave personalizada
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ed825f44923d3fe86cc410397747b50a1f2c681
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425964"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="69538-103">tipo de recurso de extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="69538-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="69538-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="69538-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="69538-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="69538-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69538-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="69538-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69538-107">Definição de uso estendido de chave personalizada</span><span class="sxs-lookup"><span data-stu-id="69538-107">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="69538-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69538-108">Properties</span></span>
|<span data-ttu-id="69538-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69538-109">Property</span></span>|<span data-ttu-id="69538-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="69538-110">Type</span></span>|<span data-ttu-id="69538-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="69538-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69538-112">name</span><span class="sxs-lookup"><span data-stu-id="69538-112">name</span></span>|<span data-ttu-id="69538-113">String</span><span class="sxs-lookup"><span data-stu-id="69538-113">String</span></span>|<span data-ttu-id="69538-114">Nome do uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="69538-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="69538-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="69538-115">objectIdentifier</span></span>|<span data-ttu-id="69538-116">String</span><span class="sxs-lookup"><span data-stu-id="69538-116">String</span></span>|<span data-ttu-id="69538-117">Identificador de objeto de uso da chave de estendido</span><span class="sxs-lookup"><span data-stu-id="69538-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="69538-118">Relações</span><span class="sxs-lookup"><span data-stu-id="69538-118">Relationships</span></span>
<span data-ttu-id="69538-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69538-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69538-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69538-120">JSON Representation</span></span>
<span data-ttu-id="69538-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69538-121">Here is a JSON representation of the resource.</span></span>
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




