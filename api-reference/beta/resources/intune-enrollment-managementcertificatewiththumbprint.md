---
title: tipo de recurso managementCertificateWithThumbprint
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e28bc8c4bbf6b4f0b1309c1241b054aa08445e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524700"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="80c21-103">tipo de recurso managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="80c21-103">managementCertificateWithThumbprint resource type</span></span>

<span data-ttu-id="80c21-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="80c21-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80c21-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="80c21-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80c21-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80c21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80c21-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="80c21-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="80c21-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80c21-108">Properties</span></span>
|<span data-ttu-id="80c21-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80c21-109">Property</span></span>|<span data-ttu-id="80c21-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="80c21-110">Type</span></span>|<span data-ttu-id="80c21-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="80c21-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80c21-112">identificação</span><span class="sxs-lookup"><span data-stu-id="80c21-112">thumbprint</span></span>|<span data-ttu-id="80c21-113">String</span><span class="sxs-lookup"><span data-stu-id="80c21-113">String</span></span>|<span data-ttu-id="80c21-114">A impressão digital do certificado de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="80c21-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="80c21-115">certificado</span><span class="sxs-lookup"><span data-stu-id="80c21-115">certificate</span></span>|<span data-ttu-id="80c21-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80c21-116">String</span></span>|<span data-ttu-id="80c21-117">O certificado de gerenciamento codificado base 64</span><span class="sxs-lookup"><span data-stu-id="80c21-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="80c21-118">Relações</span><span class="sxs-lookup"><span data-stu-id="80c21-118">Relationships</span></span>
<span data-ttu-id="80c21-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80c21-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80c21-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80c21-120">JSON Representation</span></span>
<span data-ttu-id="80c21-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80c21-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCertificateWithThumbprint",
  "thumbprint": "String",
  "certificate": "String"
}
```



