---
title: Tipo de recurso connectionInfo
description: O objeto connectionInfo define as informações de conexão usadas para se comunicar com um recurso.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 454dc7fcd045bb91819b39ad30f603191bab8380
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137699"
---
# <a name="connectioninfo-resource-type"></a><span data-ttu-id="f1c2f-103">Tipo de recurso connectionInfo</span><span class="sxs-lookup"><span data-stu-id="f1c2f-103">connectionInfo resource type</span></span>

<span data-ttu-id="f1c2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1c2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1c2f-105">O objeto connectionInfo define o localizador de recursos usado para se comunicar com um recurso no Gerenciamento de Direitos do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1c2f-105">The connectionInfo object defines the resource locator that is used to communicate with a resource in Azure AD Entitlement Management.</span></span>

## <a name="properties"></a><span data-ttu-id="f1c2f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1c2f-106">Properties</span></span>
|<span data-ttu-id="f1c2f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1c2f-107">Property</span></span>|<span data-ttu-id="f1c2f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1c2f-108">Type</span></span>|<span data-ttu-id="f1c2f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1c2f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1c2f-110">url</span><span class="sxs-lookup"><span data-stu-id="f1c2f-110">url</span></span>|<span data-ttu-id="f1c2f-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1c2f-111">String</span></span>|<span data-ttu-id="f1c2f-112">O ponto de extremidade usado pelo Gerenciamento de Direitos para se comunicar com o recurso do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="f1c2f-112">The endpoint that is used by Entitlement Management to communicate with the access package resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1c2f-113">Relações</span><span class="sxs-lookup"><span data-stu-id="f1c2f-113">Relationships</span></span>
<span data-ttu-id="f1c2f-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f1c2f-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1c2f-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1c2f-115">JSON representation</span></span>
<span data-ttu-id="f1c2f-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1c2f-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.connectionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.connectionInfo",
  "url": "String"
}
```
