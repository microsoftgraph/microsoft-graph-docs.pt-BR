---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a475f32d4572b0aa8ed2a52befc7a58eb6077253
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541162"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="7b78a-103">tipo de enumeração firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="7b78a-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="7b78a-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7b78a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b78a-105">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="7b78a-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="7b78a-106">Membros</span><span class="sxs-lookup"><span data-stu-id="7b78a-106">Members</span></span>
|<span data-ttu-id="7b78a-107">Membro</span><span class="sxs-lookup"><span data-stu-id="7b78a-107">Member</span></span>|<span data-ttu-id="7b78a-108">Valor</span><span class="sxs-lookup"><span data-stu-id="7b78a-108">Value</span></span>|<span data-ttu-id="7b78a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b78a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b78a-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="7b78a-110">deviceDefault</span></span>|<span data-ttu-id="7b78a-111">,0</span><span class="sxs-lookup"><span data-stu-id="7b78a-111">0</span></span>|<span data-ttu-id="7b78a-112">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="7b78a-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="7b78a-113">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7b78a-113">none</span></span>|<span data-ttu-id="7b78a-114">1 </span><span class="sxs-lookup"><span data-stu-id="7b78a-114">1</span></span>|<span data-ttu-id="7b78a-115">Não verificar a lista de certificados revogados</span><span class="sxs-lookup"><span data-stu-id="7b78a-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="7b78a-116">Houve</span><span class="sxs-lookup"><span data-stu-id="7b78a-116">attempt</span></span>|<span data-ttu-id="7b78a-117">2 </span><span class="sxs-lookup"><span data-stu-id="7b78a-117">2</span></span>|<span data-ttu-id="7b78a-118">Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação</span><span class="sxs-lookup"><span data-stu-id="7b78a-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="7b78a-119">precisa</span><span class="sxs-lookup"><span data-stu-id="7b78a-119">require</span></span>|<span data-ttu-id="7b78a-120">3 </span><span class="sxs-lookup"><span data-stu-id="7b78a-120">3</span></span>|<span data-ttu-id="7b78a-121">Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado</span><span class="sxs-lookup"><span data-stu-id="7b78a-121">Require a successful CRL check before allowing a certificate</span></span>|



