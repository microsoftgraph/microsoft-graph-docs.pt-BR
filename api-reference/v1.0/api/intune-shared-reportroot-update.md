---
title: Atualizar reportRoot
description: Atualizar as propriedades de um objeto reportRoot.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ba6c192b69975eef2f60b09f5bb2fc43e43d51b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885187"
---
# <a name="update-reportroot"></a><span data-ttu-id="6b7e7-103">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="6b7e7-103">Update reportRoot</span></span>

> <span data-ttu-id="6b7e7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6b7e7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b7e7-105">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="6b7e7-105">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6b7e7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6b7e7-106">Prerequisites</span></span>
<span data-ttu-id="6b7e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b7e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b7e7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b7e7-109">Permission type</span></span>|<span data-ttu-id="6b7e7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6b7e7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b7e7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b7e7-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6b7e7-112">&nbsp;&nbsp; Configuração de dispositivo</span><span class="sxs-lookup"><span data-stu-id="6b7e7-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="6b7e7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b7e7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="6b7e7-114">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="6b7e7-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="6b7e7-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b7e7-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6b7e7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b7e7-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b7e7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b7e7-117">Not supported.</span></span>|
|<span data-ttu-id="6b7e7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b7e7-118">Application</span></span>|<span data-ttu-id="6b7e7-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b7e7-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b7e7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b7e7-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="6b7e7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b7e7-121">Request headers</span></span>
|<span data-ttu-id="6b7e7-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b7e7-122">Header</span></span>|<span data-ttu-id="6b7e7-123">Valor</span><span class="sxs-lookup"><span data-stu-id="6b7e7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b7e7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b7e7-124">Authorization</span></span>|<span data-ttu-id="6b7e7-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b7e7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b7e7-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6b7e7-126">Accept</span></span>|<span data-ttu-id="6b7e7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6b7e7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b7e7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b7e7-128">Request body</span></span>
<span data-ttu-id="6b7e7-129">No corpo da solicitação, forneça uma representação JSON do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="6b7e7-129">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="6b7e7-130">A tabela a seguir mostra as propriedades que são necessárias ao criar [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="6b7e7-130">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="6b7e7-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b7e7-131">Property</span></span>|<span data-ttu-id="6b7e7-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b7e7-132">Type</span></span>|<span data-ttu-id="6b7e7-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b7e7-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b7e7-134">id</span><span class="sxs-lookup"><span data-stu-id="6b7e7-134">id</span></span>|<span data-ttu-id="6b7e7-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b7e7-135">String</span></span>|<span data-ttu-id="6b7e7-136">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="6b7e7-136">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="6b7e7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b7e7-137">Response</span></span>
<span data-ttu-id="6b7e7-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b7e7-138">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b7e7-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b7e7-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="6b7e7-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b7e7-140">Request</span></span>
<span data-ttu-id="6b7e7-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b7e7-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="6b7e7-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b7e7-142">Response</span></span>
<span data-ttu-id="6b7e7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b7e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```








