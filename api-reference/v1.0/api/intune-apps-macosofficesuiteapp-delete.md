---
title: Excluir macOSOfficeSuiteApp
description: Exclui macOSOfficeSuiteApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3202876069df7b324b300a397b338bbd46e14c9d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754445"
---
# <a name="delete-macosofficesuiteapp"></a><span data-ttu-id="3da1f-103">Excluir macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="3da1f-103">Delete macOSOfficeSuiteApp</span></span>

<span data-ttu-id="3da1f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3da1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3da1f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3da1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3da1f-106">Exclui [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="3da1f-106">Deletes a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3da1f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3da1f-107">Prerequisites</span></span>
<span data-ttu-id="3da1f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3da1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3da1f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3da1f-110">Permission type</span></span>|<span data-ttu-id="3da1f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3da1f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3da1f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3da1f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3da1f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3da1f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3da1f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3da1f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3da1f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3da1f-115">Not supported.</span></span>|
|<span data-ttu-id="3da1f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3da1f-116">Application</span></span>|<span data-ttu-id="3da1f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3da1f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3da1f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3da1f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="3da1f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3da1f-119">Request headers</span></span>
|<span data-ttu-id="3da1f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3da1f-120">Header</span></span>|<span data-ttu-id="3da1f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3da1f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3da1f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3da1f-122">Authorization</span></span>|<span data-ttu-id="3da1f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3da1f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3da1f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3da1f-124">Accept</span></span>|<span data-ttu-id="3da1f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3da1f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3da1f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3da1f-126">Request body</span></span>
<span data-ttu-id="3da1f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3da1f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3da1f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3da1f-128">Response</span></span>
<span data-ttu-id="3da1f-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3da1f-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3da1f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3da1f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3da1f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3da1f-131">Request</span></span>
<span data-ttu-id="3da1f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3da1f-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="3da1f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3da1f-133">Response</span></span>
<span data-ttu-id="3da1f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3da1f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




