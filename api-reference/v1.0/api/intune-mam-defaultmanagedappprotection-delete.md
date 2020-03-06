---
title: Excluir defaultManagedAppProtection
description: Exclui defaultManagedAppProtection.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 21db051c5dea4de58009ed3841049e48faf4d93b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513284"
---
# <a name="delete-defaultmanagedappprotection"></a><span data-ttu-id="b3df5-103">Excluir defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="b3df5-103">Delete defaultManagedAppProtection</span></span>

<span data-ttu-id="b3df5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3df5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3df5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b3df5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3df5-106">Exclui [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="b3df5-106">Deletes a [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3df5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b3df5-107">Prerequisites</span></span>
<span data-ttu-id="b3df5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3df5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3df5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3df5-110">Permission type</span></span>|<span data-ttu-id="b3df5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b3df5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3df5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3df5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3df5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3df5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b3df5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3df5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3df5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3df5-115">Not supported.</span></span>|
|<span data-ttu-id="b3df5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3df5-116">Application</span></span>|<span data-ttu-id="b3df5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3df5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3df5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3df5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="b3df5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3df5-119">Request headers</span></span>
|<span data-ttu-id="b3df5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3df5-120">Header</span></span>|<span data-ttu-id="b3df5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b3df5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3df5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3df5-122">Authorization</span></span>|<span data-ttu-id="b3df5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3df5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3df5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b3df5-124">Accept</span></span>|<span data-ttu-id="b3df5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b3df5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3df5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3df5-126">Request body</span></span>
<span data-ttu-id="b3df5-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3df5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3df5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3df5-128">Response</span></span>
<span data-ttu-id="b3df5-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b3df5-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b3df5-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3df5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3df5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3df5-131">Request</span></span>
<span data-ttu-id="b3df5-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3df5-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="b3df5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3df5-133">Response</span></span>
<span data-ttu-id="b3df5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3df5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




