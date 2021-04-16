---
title: Atualizar reportRoot
description: Atualizar as propriedades de um objeto reportRoot.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a45d6ff11476ec50f3c672455bceab8f4f5ffca5
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866199"
---
# <a name="update-reportroot"></a><span data-ttu-id="ae525-103">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="ae525-103">Update reportRoot</span></span>

<span data-ttu-id="ae525-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae525-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae525-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ae525-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae525-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ae525-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae525-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae525-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae525-108">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="ae525-108">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ae525-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae525-109">Prerequisites</span></span>
<span data-ttu-id="ae525-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae525-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae525-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae525-112">Permission type</span></span>|<span data-ttu-id="ae525-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae525-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae525-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae525-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ae525-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ae525-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ae525-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae525-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="ae525-117">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="ae525-117">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="ae525-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae525-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ae525-119">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae525-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae525-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae525-120">Not supported.</span></span>|
|<span data-ttu-id="ae525-121">Application</span><span class="sxs-lookup"><span data-stu-id="ae525-121">Application</span></span>||
| <span data-ttu-id="ae525-122">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ae525-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ae525-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae525-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="ae525-124">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="ae525-124">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="ae525-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae525-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae525-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae525-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="ae525-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae525-127">Request headers</span></span>
|<span data-ttu-id="ae525-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae525-128">Header</span></span>|<span data-ttu-id="ae525-129">Valor</span><span class="sxs-lookup"><span data-stu-id="ae525-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae525-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae525-130">Authorization</span></span>|<span data-ttu-id="ae525-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae525-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae525-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae525-132">Accept</span></span>|<span data-ttu-id="ae525-133">application/json</span><span class="sxs-lookup"><span data-stu-id="ae525-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae525-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae525-134">Request body</span></span>
<span data-ttu-id="ae525-135">No corpo da solicitação, forneça uma representação JSON do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="ae525-135">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="ae525-136">A tabela a seguir mostra as propriedades que são necessárias ao criar [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="ae525-136">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="ae525-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae525-137">Property</span></span>|<span data-ttu-id="ae525-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae525-138">Type</span></span>|<span data-ttu-id="ae525-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae525-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae525-140">id</span><span class="sxs-lookup"><span data-stu-id="ae525-140">id</span></span>|<span data-ttu-id="ae525-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae525-141">String</span></span>|<span data-ttu-id="ae525-142">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="ae525-142">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="ae525-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae525-143">Response</span></span>
<span data-ttu-id="ae525-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae525-144">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae525-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae525-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="ae525-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae525-146">Request</span></span>
<span data-ttu-id="ae525-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae525-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="ae525-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae525-148">Response</span></span>
<span data-ttu-id="ae525-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae525-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```










