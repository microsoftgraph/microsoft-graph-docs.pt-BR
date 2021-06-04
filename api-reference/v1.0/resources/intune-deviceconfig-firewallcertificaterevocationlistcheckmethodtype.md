---
title: tipo de número firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 779cfe8b8576d475df62ed112709aa0c2e9b6c63
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754724"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="02d8d-103">tipo de número firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="02d8d-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="02d8d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02d8d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02d8d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02d8d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02d8d-106">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="02d8d-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="02d8d-107">Membros</span><span class="sxs-lookup"><span data-stu-id="02d8d-107">Members</span></span>
|<span data-ttu-id="02d8d-108">Membro</span><span class="sxs-lookup"><span data-stu-id="02d8d-108">Member</span></span>|<span data-ttu-id="02d8d-109">Valor</span><span class="sxs-lookup"><span data-stu-id="02d8d-109">Value</span></span>|<span data-ttu-id="02d8d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="02d8d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02d8d-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="02d8d-111">deviceDefault</span></span>|<span data-ttu-id="02d8d-112">0</span><span class="sxs-lookup"><span data-stu-id="02d8d-112">0</span></span>|<span data-ttu-id="02d8d-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="02d8d-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="02d8d-114">nenhuma</span><span class="sxs-lookup"><span data-stu-id="02d8d-114">none</span></span>|<span data-ttu-id="02d8d-115">1</span><span class="sxs-lookup"><span data-stu-id="02d8d-115">1</span></span>|<span data-ttu-id="02d8d-116">Não verificar lista de revogação de certificado</span><span class="sxs-lookup"><span data-stu-id="02d8d-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="02d8d-117">tentativa</span><span class="sxs-lookup"><span data-stu-id="02d8d-117">attempt</span></span>|<span data-ttu-id="02d8d-118">2</span><span class="sxs-lookup"><span data-stu-id="02d8d-118">2</span></span>|<span data-ttu-id="02d8d-119">Tente verificar CRL e permitir um certificado somente se o certificado for confirmado pela verificação</span><span class="sxs-lookup"><span data-stu-id="02d8d-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="02d8d-120">require</span><span class="sxs-lookup"><span data-stu-id="02d8d-120">require</span></span>|<span data-ttu-id="02d8d-121">3</span><span class="sxs-lookup"><span data-stu-id="02d8d-121">3</span></span>|<span data-ttu-id="02d8d-122">Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado</span><span class="sxs-lookup"><span data-stu-id="02d8d-122">Require a successful CRL check before allowing a certificate</span></span>|




