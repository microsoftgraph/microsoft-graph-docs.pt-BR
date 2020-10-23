---
title: tipo de enumeração emailCertificateType
description: Fontes de certificado com suporte para assinatura e criptografia de email.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 691923c70c89d2f29cb45f6f3a994bbc919a7d56
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705971"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="e6ba7-103">tipo de enumeração emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="e6ba7-103">emailCertificateType enum type</span></span>

<span data-ttu-id="e6ba7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6ba7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6ba7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e6ba7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6ba7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6ba7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6ba7-107">Fontes de certificado com suporte para assinatura e criptografia de email.</span><span class="sxs-lookup"><span data-stu-id="e6ba7-107">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="e6ba7-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e6ba7-108">Members</span></span>
|<span data-ttu-id="e6ba7-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e6ba7-109">Member</span></span>|<span data-ttu-id="e6ba7-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e6ba7-110">Value</span></span>|<span data-ttu-id="e6ba7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6ba7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6ba7-112">none</span><span class="sxs-lookup"><span data-stu-id="e6ba7-112">none</span></span>|<span data-ttu-id="e6ba7-113">,0</span><span class="sxs-lookup"><span data-stu-id="e6ba7-113">0</span></span>|<span data-ttu-id="e6ba7-114">Não use um certificado como fonte.</span><span class="sxs-lookup"><span data-stu-id="e6ba7-114">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="e6ba7-115">certificado</span><span class="sxs-lookup"><span data-stu-id="e6ba7-115">certificate</span></span>|<span data-ttu-id="e6ba7-116">1</span><span class="sxs-lookup"><span data-stu-id="e6ba7-116">1</span></span>|<span data-ttu-id="e6ba7-117">Usar um certificado para a fonte do certificado.</span><span class="sxs-lookup"><span data-stu-id="e6ba7-117">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="e6ba7-118">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="e6ba7-118">derivedCredential</span></span>|<span data-ttu-id="e6ba7-119">duas</span><span class="sxs-lookup"><span data-stu-id="e6ba7-119">2</span></span>|<span data-ttu-id="e6ba7-120">Use uma credencial derivada para a fonte do certificado.</span><span class="sxs-lookup"><span data-stu-id="e6ba7-120">Use a derived credential for certificate source.</span></span>|





