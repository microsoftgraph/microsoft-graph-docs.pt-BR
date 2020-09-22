---
title: tipo de enumeração emailCertificateType
description: Fontes de certificado com suporte para assinatura e criptografia de email.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b5fe1392d09576de4d0154d941d87293f87615bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095258"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="19b2b-103">tipo de enumeração emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="19b2b-103">emailCertificateType enum type</span></span>

<span data-ttu-id="19b2b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19b2b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19b2b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="19b2b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19b2b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="19b2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19b2b-107">Fontes de certificado com suporte para assinatura e criptografia de email.</span><span class="sxs-lookup"><span data-stu-id="19b2b-107">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="19b2b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="19b2b-108">Members</span></span>
|<span data-ttu-id="19b2b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="19b2b-109">Member</span></span>|<span data-ttu-id="19b2b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="19b2b-110">Value</span></span>|<span data-ttu-id="19b2b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="19b2b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19b2b-112">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="19b2b-112">none</span></span>|<span data-ttu-id="19b2b-113">,0</span><span class="sxs-lookup"><span data-stu-id="19b2b-113">0</span></span>|<span data-ttu-id="19b2b-114">Não use um certificado como fonte.</span><span class="sxs-lookup"><span data-stu-id="19b2b-114">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="19b2b-115">certificado</span><span class="sxs-lookup"><span data-stu-id="19b2b-115">certificate</span></span>|<span data-ttu-id="19b2b-116">1 </span><span class="sxs-lookup"><span data-stu-id="19b2b-116">1</span></span>|<span data-ttu-id="19b2b-117">Usar um certificado para a fonte do certificado.</span><span class="sxs-lookup"><span data-stu-id="19b2b-117">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="19b2b-118">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="19b2b-118">derivedCredential</span></span>|<span data-ttu-id="19b2b-119">2 </span><span class="sxs-lookup"><span data-stu-id="19b2b-119">2</span></span>|<span data-ttu-id="19b2b-120">Use uma credencial derivada para a fonte do certificado.</span><span class="sxs-lookup"><span data-stu-id="19b2b-120">Use a derived credential for certificate source.</span></span>|






