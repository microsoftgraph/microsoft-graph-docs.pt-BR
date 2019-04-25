---
title: Atualizar reportRoot
description: Atualizar as propriedades de um objeto reportRoot.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0039490379054ddb98c687957c1af0462a2e7f02
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576815"
---
# <a name="update-reportroot"></a><span data-ttu-id="d8034-103">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="d8034-103">Update reportRoot</span></span>

> <span data-ttu-id="d8034-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8034-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8034-105">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="d8034-105">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8034-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8034-106">Prerequisites</span></span>
<span data-ttu-id="d8034-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8034-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8034-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8034-109">Permission type</span></span>|<span data-ttu-id="d8034-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8034-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8034-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8034-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d8034-112">&nbsp;&nbsp; Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d8034-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="d8034-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8034-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="d8034-114">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="d8034-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="d8034-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8034-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d8034-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8034-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8034-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8034-117">Not supported.</span></span>|
|<span data-ttu-id="d8034-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8034-118">Application</span></span>|<span data-ttu-id="d8034-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8034-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8034-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8034-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="d8034-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8034-121">Request headers</span></span>
|<span data-ttu-id="d8034-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8034-122">Header</span></span>|<span data-ttu-id="d8034-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d8034-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8034-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8034-124">Authorization</span></span>|<span data-ttu-id="d8034-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8034-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8034-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8034-126">Accept</span></span>|<span data-ttu-id="d8034-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d8034-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8034-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8034-128">Request body</span></span>
<span data-ttu-id="d8034-129">No corpo da solicitação, forneça uma representação JSON do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="d8034-129">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="d8034-130">A tabela a seguir mostra as propriedades que são necessárias ao criar [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="d8034-130">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="d8034-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8034-131">Property</span></span>|<span data-ttu-id="d8034-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8034-132">Type</span></span>|<span data-ttu-id="d8034-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8034-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8034-134">id</span><span class="sxs-lookup"><span data-stu-id="d8034-134">id</span></span>|<span data-ttu-id="d8034-135">String</span><span class="sxs-lookup"><span data-stu-id="d8034-135">String</span></span>|<span data-ttu-id="d8034-136">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="d8034-136">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="d8034-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8034-137">Response</span></span>
<span data-ttu-id="d8034-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8034-138">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8034-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8034-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8034-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8034-140">Request</span></span>
<span data-ttu-id="d8034-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8034-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="d8034-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8034-142">Response</span></span>
<span data-ttu-id="d8034-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8034-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```








