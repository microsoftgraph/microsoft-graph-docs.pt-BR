---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 52377b6b94357edfdd5c3c9945f3aefe30695968
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030032"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="fd271-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="fd271-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="fd271-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd271-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd271-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fd271-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd271-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fd271-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd271-107">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="fd271-107">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="fd271-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd271-108">Properties</span></span>
|<span data-ttu-id="fd271-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd271-109">Property</span></span>|<span data-ttu-id="fd271-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd271-110">Type</span></span>|<span data-ttu-id="fd271-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd271-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd271-112">SubjectName</span><span class="sxs-lookup"><span data-stu-id="fd271-112">subjectName</span></span>|<span data-ttu-id="fd271-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd271-113">String</span></span>|<span data-ttu-id="fd271-114">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="fd271-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="fd271-115">description</span><span class="sxs-lookup"><span data-stu-id="fd271-115">description</span></span>|<span data-ttu-id="fd271-116">String</span><span class="sxs-lookup"><span data-stu-id="fd271-116">String</span></span>|<span data-ttu-id="fd271-117">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="fd271-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="fd271-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fd271-118">expirationDateTime</span></span>|<span data-ttu-id="fd271-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd271-119">DateTimeOffset</span></span>|<span data-ttu-id="fd271-120">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="fd271-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="fd271-121">certificado</span><span class="sxs-lookup"><span data-stu-id="fd271-121">certificate</span></span>|<span data-ttu-id="fd271-122">Binário</span><span class="sxs-lookup"><span data-stu-id="fd271-122">Binary</span></span>|<span data-ttu-id="fd271-123">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="fd271-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd271-124">Relações</span><span class="sxs-lookup"><span data-stu-id="fd271-124">Relationships</span></span>
<span data-ttu-id="fd271-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fd271-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd271-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd271-126">JSON Representation</span></span>
<span data-ttu-id="fd271-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fd271-127">Here is a JSON representation of the resource.</span></span>
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






