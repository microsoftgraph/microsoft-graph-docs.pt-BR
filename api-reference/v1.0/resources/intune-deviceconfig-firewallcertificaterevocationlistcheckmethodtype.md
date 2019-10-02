---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 42f470d7f3d8ef29a69ba8f1cd4f76ddc0f77e96
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359268"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="84e86-103">tipo de enumeração firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="84e86-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="84e86-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84e86-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84e86-105">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="84e86-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="84e86-106">Membros</span><span class="sxs-lookup"><span data-stu-id="84e86-106">Members</span></span>
|<span data-ttu-id="84e86-107">Membro</span><span class="sxs-lookup"><span data-stu-id="84e86-107">Member</span></span>|<span data-ttu-id="84e86-108">Valor</span><span class="sxs-lookup"><span data-stu-id="84e86-108">Value</span></span>|<span data-ttu-id="84e86-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="84e86-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84e86-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="84e86-110">deviceDefault</span></span>|<span data-ttu-id="84e86-111">,0</span><span class="sxs-lookup"><span data-stu-id="84e86-111">0</span></span>|<span data-ttu-id="84e86-112">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="84e86-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="84e86-113">none</span><span class="sxs-lookup"><span data-stu-id="84e86-113">none</span></span>|<span data-ttu-id="84e86-114">1</span><span class="sxs-lookup"><span data-stu-id="84e86-114">1</span></span>|<span data-ttu-id="84e86-115">Não verificar a lista de certificados revogados</span><span class="sxs-lookup"><span data-stu-id="84e86-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="84e86-116">Houve</span><span class="sxs-lookup"><span data-stu-id="84e86-116">attempt</span></span>|<span data-ttu-id="84e86-117">duas</span><span class="sxs-lookup"><span data-stu-id="84e86-117">2</span></span>|<span data-ttu-id="84e86-118">Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação</span><span class="sxs-lookup"><span data-stu-id="84e86-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="84e86-119">precisa</span><span class="sxs-lookup"><span data-stu-id="84e86-119">require</span></span>|<span data-ttu-id="84e86-120">3D</span><span class="sxs-lookup"><span data-stu-id="84e86-120">3</span></span>|<span data-ttu-id="84e86-121">Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado</span><span class="sxs-lookup"><span data-stu-id="84e86-121">Require a successful CRL check before allowing a certificate</span></span>|




