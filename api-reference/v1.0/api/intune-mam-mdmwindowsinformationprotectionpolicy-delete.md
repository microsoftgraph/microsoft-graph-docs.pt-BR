---
title: Excluir mdmWindowsInformationProtectionPolicy
description: Exclui mdmWindowsInformationProtectionPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d8b5a20dfc2e47d332315c8e126e00b10327588
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018173"
---
# <a name="delete-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="3b380-103">Excluir mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="3b380-103">Delete mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="3b380-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b380-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b380-105">Exclui [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b380-105">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b380-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b380-106">Prerequisites</span></span>
<span data-ttu-id="3b380-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b380-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b380-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b380-109">Permission type</span></span>|<span data-ttu-id="3b380-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b380-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b380-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b380-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3b380-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b380-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3b380-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b380-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b380-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b380-114">Not supported.</span></span>|
|<span data-ttu-id="3b380-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b380-115">Application</span></span>|<span data-ttu-id="3b380-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b380-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b380-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b380-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="3b380-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b380-118">Request headers</span></span>
|<span data-ttu-id="3b380-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b380-119">Header</span></span>|<span data-ttu-id="3b380-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3b380-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b380-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b380-121">Authorization</span></span>|<span data-ttu-id="3b380-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b380-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b380-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b380-123">Accept</span></span>|<span data-ttu-id="3b380-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3b380-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b380-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b380-125">Request body</span></span>
<span data-ttu-id="3b380-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b380-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b380-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b380-127">Response</span></span>
<span data-ttu-id="3b380-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3b380-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3b380-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b380-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b380-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b380-130">Request</span></span>
<span data-ttu-id="3b380-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b380-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="3b380-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b380-132">Response</span></span>
<span data-ttu-id="3b380-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b380-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



