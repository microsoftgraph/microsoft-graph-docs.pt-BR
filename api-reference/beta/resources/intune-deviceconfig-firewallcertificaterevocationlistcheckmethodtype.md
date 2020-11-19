---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3c1c9e4ae9068f6dc9d754da93a30979367e7587
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294498"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="c7bbe-103">tipo de enumeração firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="c7bbe-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="c7bbe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7bbe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7bbe-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7bbe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7bbe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7bbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7bbe-107">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="c7bbe-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="c7bbe-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c7bbe-108">Members</span></span>
|<span data-ttu-id="c7bbe-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c7bbe-109">Member</span></span>|<span data-ttu-id="c7bbe-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c7bbe-110">Value</span></span>|<span data-ttu-id="c7bbe-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7bbe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7bbe-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c7bbe-112">deviceDefault</span></span>|<span data-ttu-id="c7bbe-113">,0</span><span class="sxs-lookup"><span data-stu-id="c7bbe-113">0</span></span>|<span data-ttu-id="c7bbe-114">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="c7bbe-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="c7bbe-115">nenhum</span><span class="sxs-lookup"><span data-stu-id="c7bbe-115">none</span></span>|<span data-ttu-id="c7bbe-116">1</span><span class="sxs-lookup"><span data-stu-id="c7bbe-116">1</span></span>|<span data-ttu-id="c7bbe-117">Não verificar a lista de certificados revogados</span><span class="sxs-lookup"><span data-stu-id="c7bbe-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="c7bbe-118">Houve</span><span class="sxs-lookup"><span data-stu-id="c7bbe-118">attempt</span></span>|<span data-ttu-id="c7bbe-119">duas</span><span class="sxs-lookup"><span data-stu-id="c7bbe-119">2</span></span>|<span data-ttu-id="c7bbe-120">Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação</span><span class="sxs-lookup"><span data-stu-id="c7bbe-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="c7bbe-121">precisa</span><span class="sxs-lookup"><span data-stu-id="c7bbe-121">require</span></span>|<span data-ttu-id="c7bbe-122">3D</span><span class="sxs-lookup"><span data-stu-id="c7bbe-122">3</span></span>|<span data-ttu-id="c7bbe-123">Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado</span><span class="sxs-lookup"><span data-stu-id="c7bbe-123">Require a successful CRL check before allowing a certificate</span></span>|




