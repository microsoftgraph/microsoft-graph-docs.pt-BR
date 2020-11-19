---
title: tipo de recurso androidEnrollmentCompanyCode
description: Uma classe para manter os dados de registro Specialty usados para registrar-se por meio da API de gerenciamento do Android do Google, como token, URL e conteúdo de código QR
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 986c298abfc9e86c32c57cb5cdaa9c31ee159791
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49282255"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="f8aff-103">tipo de recurso androidEnrollmentCompanyCode</span><span class="sxs-lookup"><span data-stu-id="f8aff-103">androidEnrollmentCompanyCode resource type</span></span>

<span data-ttu-id="f8aff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8aff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8aff-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8aff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8aff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8aff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8aff-107">Uma classe para manter os dados de registro Specialty usados para registrar-se por meio da API de gerenciamento do Android do Google, como token, URL e conteúdo de código QR</span><span class="sxs-lookup"><span data-stu-id="f8aff-107">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="f8aff-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8aff-108">Properties</span></span>
|<span data-ttu-id="f8aff-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8aff-109">Property</span></span>|<span data-ttu-id="f8aff-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8aff-110">Type</span></span>|<span data-ttu-id="f8aff-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8aff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8aff-112">enrollmentToken</span><span class="sxs-lookup"><span data-stu-id="f8aff-112">enrollmentToken</span></span>|<span data-ttu-id="f8aff-113">String</span><span class="sxs-lookup"><span data-stu-id="f8aff-113">String</span></span>|<span data-ttu-id="f8aff-114">Token de registro usado pelo usuário para registrar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f8aff-114">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="f8aff-115">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="f8aff-115">qrCodeContent</span></span>|<span data-ttu-id="f8aff-116">String</span><span class="sxs-lookup"><span data-stu-id="f8aff-116">String</span></span>|<span data-ttu-id="f8aff-117">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="f8aff-117">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="f8aff-118">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="f8aff-118">qrCodeImage</span></span>|[<span data-ttu-id="f8aff-119">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f8aff-119">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f8aff-120">Código QR gerado para o token.</span><span class="sxs-lookup"><span data-stu-id="f8aff-120">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8aff-121">Relações</span><span class="sxs-lookup"><span data-stu-id="f8aff-121">Relationships</span></span>
<span data-ttu-id="f8aff-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f8aff-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8aff-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f8aff-123">JSON Representation</span></span>
<span data-ttu-id="f8aff-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f8aff-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnrollmentCompanyCode",
  "enrollmentToken": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```




