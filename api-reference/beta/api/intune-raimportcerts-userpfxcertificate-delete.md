---
title: Excluir userPFXCertificate
description: Exclui userPFXCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6f180fc9e7c15a65315f9faf9bcecb9764e3d7bb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49270033"
---
# <a name="delete-userpfxcertificate"></a><span data-ttu-id="463ed-103">Excluir userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="463ed-103">Delete userPFXCertificate</span></span>

<span data-ttu-id="463ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="463ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="463ed-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="463ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="463ed-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="463ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="463ed-107">Exclui [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="463ed-107">Deletes a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="463ed-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="463ed-108">Prerequisites</span></span>
<span data-ttu-id="463ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="463ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="463ed-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="463ed-111">Permission type</span></span>|<span data-ttu-id="463ed-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="463ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="463ed-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="463ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="463ed-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="463ed-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="463ed-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="463ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="463ed-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="463ed-116">Not supported.</span></span>|
|<span data-ttu-id="463ed-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="463ed-117">Application</span></span>|<span data-ttu-id="463ed-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="463ed-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="463ed-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="463ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="463ed-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="463ed-120">Request headers</span></span>
|<span data-ttu-id="463ed-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="463ed-121">Header</span></span>|<span data-ttu-id="463ed-122">Valor</span><span class="sxs-lookup"><span data-stu-id="463ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="463ed-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="463ed-123">Authorization</span></span>|<span data-ttu-id="463ed-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="463ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="463ed-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="463ed-125">Accept</span></span>|<span data-ttu-id="463ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="463ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="463ed-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="463ed-127">Request body</span></span>
<span data-ttu-id="463ed-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="463ed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="463ed-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="463ed-129">Response</span></span>
<span data-ttu-id="463ed-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="463ed-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="463ed-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="463ed-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="463ed-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="463ed-132">Request</span></span>
<span data-ttu-id="463ed-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="463ed-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

### <a name="response"></a><span data-ttu-id="463ed-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="463ed-134">Response</span></span>
<span data-ttu-id="463ed-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="463ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




