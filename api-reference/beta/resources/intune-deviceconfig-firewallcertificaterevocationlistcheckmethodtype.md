---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2ef4a78a7e61f18b52b322b4053ebfbfa7e54e05
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791755"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="70a01-103">tipo de enumeração firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="70a01-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="70a01-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="70a01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70a01-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="70a01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70a01-106">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="70a01-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="70a01-107">Membros</span><span class="sxs-lookup"><span data-stu-id="70a01-107">Members</span></span>
|<span data-ttu-id="70a01-108">Membro</span><span class="sxs-lookup"><span data-stu-id="70a01-108">Member</span></span>|<span data-ttu-id="70a01-109">Valor</span><span class="sxs-lookup"><span data-stu-id="70a01-109">Value</span></span>|<span data-ttu-id="70a01-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="70a01-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70a01-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="70a01-111">deviceDefault</span></span>|<span data-ttu-id="70a01-112">,0</span><span class="sxs-lookup"><span data-stu-id="70a01-112">0</span></span>|<span data-ttu-id="70a01-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="70a01-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="70a01-114">none</span><span class="sxs-lookup"><span data-stu-id="70a01-114">none</span></span>|<span data-ttu-id="70a01-115">1</span><span class="sxs-lookup"><span data-stu-id="70a01-115">1</span></span>|<span data-ttu-id="70a01-116">Não verificar a lista de certificados revogados</span><span class="sxs-lookup"><span data-stu-id="70a01-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="70a01-117">Houve</span><span class="sxs-lookup"><span data-stu-id="70a01-117">attempt</span></span>|<span data-ttu-id="70a01-118">duas</span><span class="sxs-lookup"><span data-stu-id="70a01-118">2</span></span>|<span data-ttu-id="70a01-119">Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação</span><span class="sxs-lookup"><span data-stu-id="70a01-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="70a01-120">precisa</span><span class="sxs-lookup"><span data-stu-id="70a01-120">require</span></span>|<span data-ttu-id="70a01-121">3D</span><span class="sxs-lookup"><span data-stu-id="70a01-121">3</span></span>|<span data-ttu-id="70a01-122">Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado</span><span class="sxs-lookup"><span data-stu-id="70a01-122">Require a successful CRL check before allowing a certificate</span></span>|



