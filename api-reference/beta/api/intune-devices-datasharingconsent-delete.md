---
title: Excluir dataSharingConsent
description: Exclui dataSharingConsent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9427d183e7c908b38b84ec768cc6c1d1cb33f71
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33910168"
---
# <a name="delete-datasharingconsent"></a><span data-ttu-id="88d82-103">Excluir dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="88d82-103">Delete dataSharingConsent</span></span>

> <span data-ttu-id="88d82-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88d82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88d82-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88d82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88d82-106">Exclui [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span><span class="sxs-lookup"><span data-stu-id="88d82-106">Deletes a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88d82-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88d82-107">Prerequisites</span></span>
<span data-ttu-id="88d82-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88d82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88d82-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88d82-110">Permission type</span></span>|<span data-ttu-id="88d82-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="88d82-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88d82-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88d82-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88d82-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88d82-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="88d82-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88d82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88d82-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88d82-115">Not supported.</span></span>|
|<span data-ttu-id="88d82-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88d82-116">Application</span></span>|<span data-ttu-id="88d82-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88d82-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88d82-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88d82-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="request-headers"></a><span data-ttu-id="88d82-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88d82-119">Request headers</span></span>
|<span data-ttu-id="88d82-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88d82-120">Header</span></span>|<span data-ttu-id="88d82-121">Valor</span><span class="sxs-lookup"><span data-stu-id="88d82-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88d82-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="88d82-122">Authorization</span></span>|<span data-ttu-id="88d82-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88d82-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88d82-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88d82-124">Accept</span></span>|<span data-ttu-id="88d82-125">application/json</span><span class="sxs-lookup"><span data-stu-id="88d82-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88d82-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88d82-126">Request body</span></span>
<span data-ttu-id="88d82-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88d82-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88d82-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="88d82-128">Response</span></span>
<span data-ttu-id="88d82-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="88d82-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="88d82-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88d82-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="88d82-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88d82-131">Request</span></span>
<span data-ttu-id="88d82-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88d82-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

### <a name="response"></a><span data-ttu-id="88d82-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="88d82-133">Response</span></span>
<span data-ttu-id="88d82-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88d82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




