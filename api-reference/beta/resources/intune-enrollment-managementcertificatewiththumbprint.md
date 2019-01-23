---
title: tipo de recurso de managementCertificateWithThumbprint
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 765d3b9370e4b0f5eda481883956c72bf261e65a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418852"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="0f213-103">tipo de recurso de managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="0f213-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="0f213-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="0f213-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0f213-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0f213-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f213-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0f213-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f213-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0f213-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0f213-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f213-108">Properties</span></span>
|<span data-ttu-id="0f213-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f213-109">Property</span></span>|<span data-ttu-id="0f213-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f213-110">Type</span></span>|<span data-ttu-id="0f213-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f213-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f213-112">impressão digital</span><span class="sxs-lookup"><span data-stu-id="0f213-112">thumbprint</span></span>|<span data-ttu-id="0f213-113">String</span><span class="sxs-lookup"><span data-stu-id="0f213-113">String</span></span>|<span data-ttu-id="0f213-114">A impressão digital do certificado gerenciamento</span><span class="sxs-lookup"><span data-stu-id="0f213-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="0f213-115">certificado</span><span class="sxs-lookup"><span data-stu-id="0f213-115">certificate</span></span>|<span data-ttu-id="0f213-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f213-116">String</span></span>|<span data-ttu-id="0f213-117">O certificado de gerenciamento codificada de Base 64</span><span class="sxs-lookup"><span data-stu-id="0f213-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f213-118">Relações</span><span class="sxs-lookup"><span data-stu-id="0f213-118">Relationships</span></span>
<span data-ttu-id="0f213-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0f213-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f213-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f213-120">JSON Representation</span></span>
<span data-ttu-id="0f213-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f213-121">Here is a JSON representation of the resource.</span></span>
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




