---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c3c75af9126c06693b58eb0389c4199092e69c2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373221"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="dd646-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="dd646-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="dd646-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dd646-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd646-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dd646-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd646-106">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="dd646-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="dd646-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd646-107">Properties</span></span>
|<span data-ttu-id="dd646-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd646-108">Property</span></span>|<span data-ttu-id="dd646-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd646-109">Type</span></span>|<span data-ttu-id="dd646-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd646-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd646-111">SubjectName</span><span class="sxs-lookup"><span data-stu-id="dd646-111">subjectName</span></span>|<span data-ttu-id="dd646-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd646-112">String</span></span>|<span data-ttu-id="dd646-113">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="dd646-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="dd646-114">descrição</span><span class="sxs-lookup"><span data-stu-id="dd646-114">description</span></span>|<span data-ttu-id="dd646-115">String</span><span class="sxs-lookup"><span data-stu-id="dd646-115">String</span></span>|<span data-ttu-id="dd646-116">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="dd646-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="dd646-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dd646-117">expirationDateTime</span></span>|<span data-ttu-id="dd646-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd646-118">DateTimeOffset</span></span>|<span data-ttu-id="dd646-119">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="dd646-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="dd646-120">certificado</span><span class="sxs-lookup"><span data-stu-id="dd646-120">certificate</span></span>|<span data-ttu-id="dd646-121">Binário</span><span class="sxs-lookup"><span data-stu-id="dd646-121">Binary</span></span>|<span data-ttu-id="dd646-122">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="dd646-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd646-123">Relações</span><span class="sxs-lookup"><span data-stu-id="dd646-123">Relationships</span></span>
<span data-ttu-id="dd646-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd646-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd646-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd646-125">JSON Representation</span></span>
<span data-ttu-id="dd646-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd646-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```



