---
title: Excluir auditEvent
description: Exclui auditEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b8fe9c21dd59858f61c0d5e6c79464fb9cd7c44a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32484451"
---
# <a name="delete-auditevent"></a><span data-ttu-id="49eac-103">Excluir auditEvent</span><span class="sxs-lookup"><span data-stu-id="49eac-103">Delete auditEvent</span></span>

> <span data-ttu-id="49eac-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49eac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49eac-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49eac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49eac-106">Exclui [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="49eac-106">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49eac-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49eac-107">Prerequisites</span></span>
<span data-ttu-id="49eac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49eac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49eac-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49eac-110">Permission type</span></span>|<span data-ttu-id="49eac-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49eac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49eac-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49eac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49eac-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49eac-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="49eac-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49eac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49eac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49eac-115">Not supported.</span></span>|
|<span data-ttu-id="49eac-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49eac-116">Application</span></span>|<span data-ttu-id="49eac-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49eac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49eac-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49eac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/auditEvents/{auditEventId}
```

## <a name="request-headers"></a><span data-ttu-id="49eac-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49eac-119">Request headers</span></span>
|<span data-ttu-id="49eac-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49eac-120">Header</span></span>|<span data-ttu-id="49eac-121">Valor</span><span class="sxs-lookup"><span data-stu-id="49eac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49eac-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="49eac-122">Authorization</span></span>|<span data-ttu-id="49eac-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49eac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49eac-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49eac-124">Accept</span></span>|<span data-ttu-id="49eac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49eac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49eac-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49eac-126">Request body</span></span>
<span data-ttu-id="49eac-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="49eac-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49eac-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="49eac-128">Response</span></span>
<span data-ttu-id="49eac-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="49eac-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="49eac-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49eac-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="49eac-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49eac-131">Request</span></span>
<span data-ttu-id="49eac-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49eac-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="49eac-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="49eac-133">Response</span></span>
<span data-ttu-id="49eac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49eac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





