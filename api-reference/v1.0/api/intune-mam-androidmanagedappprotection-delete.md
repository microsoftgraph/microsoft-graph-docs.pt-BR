---
title: Excluir androidManagedAppProtection
description: Excluir um androidManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0735d432da3664c2e27e663ecc5f031ac0bcec3c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263130"
---
# <a name="delete-androidmanagedappprotection"></a><span data-ttu-id="cefc4-103">Excluir androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="cefc4-103">Delete androidManagedAppProtection</span></span>

> <span data-ttu-id="cefc4-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cefc4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cefc4-105">Exclui [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="cefc4-105">Deletes a [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cefc4-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cefc4-106">Prerequisites</span></span>
<span data-ttu-id="cefc4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cefc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cefc4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cefc4-109">Permission type</span></span>|<span data-ttu-id="cefc4-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cefc4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cefc4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cefc4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cefc4-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cefc4-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cefc4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cefc4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cefc4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cefc4-114">Not supported.</span></span>|
|<span data-ttu-id="cefc4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cefc4-115">Application</span></span>|<span data-ttu-id="cefc4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cefc4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cefc4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cefc4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="cefc4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cefc4-118">Request headers</span></span>
|<span data-ttu-id="cefc4-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cefc4-119">Header</span></span>|<span data-ttu-id="cefc4-120">Valor</span><span class="sxs-lookup"><span data-stu-id="cefc4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cefc4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cefc4-121">Authorization</span></span>|<span data-ttu-id="cefc4-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cefc4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cefc4-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cefc4-123">Accept</span></span>|<span data-ttu-id="cefc4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cefc4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cefc4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cefc4-125">Request body</span></span>
<span data-ttu-id="cefc4-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cefc4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cefc4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="cefc4-127">Response</span></span>
<span data-ttu-id="cefc4-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cefc4-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cefc4-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cefc4-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="cefc4-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cefc4-130">Request</span></span>
<span data-ttu-id="cefc4-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cefc4-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="cefc4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cefc4-132">Response</span></span>
<span data-ttu-id="cefc4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cefc4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



