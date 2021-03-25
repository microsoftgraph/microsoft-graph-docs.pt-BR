---
title: Criar cartToClassAssociation
description: Crie um novo objeto cartToClassAssociation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 50d99bd3f8c00e7c3fe1e4079447243248d93776
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155831"
---
# <a name="create-carttoclassassociation"></a><span data-ttu-id="39672-103">Criar cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="39672-103">Create cartToClassAssociation</span></span>

<span data-ttu-id="39672-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39672-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39672-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="39672-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39672-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39672-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39672-107">Crie um novo [objeto cartToClassAssociation.](../resources/intune-deviceconfig-carttoclassassociation.md)</span><span class="sxs-lookup"><span data-stu-id="39672-107">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39672-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="39672-108">Prerequisites</span></span>
<span data-ttu-id="39672-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39672-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39672-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39672-111">Permission type</span></span>|<span data-ttu-id="39672-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39672-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39672-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39672-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39672-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39672-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39672-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39672-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39672-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39672-116">Not supported.</span></span>|
|<span data-ttu-id="39672-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39672-117">Application</span></span>|<span data-ttu-id="39672-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39672-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="39672-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39672-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="39672-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39672-120">Request headers</span></span>
|<span data-ttu-id="39672-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="39672-121">Header</span></span>|<span data-ttu-id="39672-122">Valor</span><span class="sxs-lookup"><span data-stu-id="39672-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39672-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="39672-123">Authorization</span></span>|<span data-ttu-id="39672-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39672-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39672-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="39672-125">Accept</span></span>|<span data-ttu-id="39672-126">application/json</span><span class="sxs-lookup"><span data-stu-id="39672-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39672-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39672-127">Request body</span></span>
<span data-ttu-id="39672-128">No corpo da solicitação, fornece uma representação JSON para o objeto cartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="39672-128">In the request body, supply a JSON representation for the cartToClassAssociation object.</span></span>

<span data-ttu-id="39672-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o cartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="39672-129">The following table shows the properties that are required when you create the cartToClassAssociation.</span></span>

|<span data-ttu-id="39672-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39672-130">Property</span></span>|<span data-ttu-id="39672-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="39672-131">Type</span></span>|<span data-ttu-id="39672-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="39672-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39672-133">id</span><span class="sxs-lookup"><span data-stu-id="39672-133">id</span></span>|<span data-ttu-id="39672-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39672-134">String</span></span>|<span data-ttu-id="39672-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="39672-135">Key of the entity.</span></span>|
|<span data-ttu-id="39672-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39672-136">createdDateTime</span></span>|<span data-ttu-id="39672-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39672-137">DateTimeOffset</span></span>|<span data-ttu-id="39672-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="39672-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="39672-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39672-139">lastModifiedDateTime</span></span>|<span data-ttu-id="39672-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39672-140">DateTimeOffset</span></span>|<span data-ttu-id="39672-141">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="39672-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="39672-142">versão</span><span class="sxs-lookup"><span data-stu-id="39672-142">version</span></span>|<span data-ttu-id="39672-143">Int32</span><span class="sxs-lookup"><span data-stu-id="39672-143">Int32</span></span>|<span data-ttu-id="39672-144">Versão do CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="39672-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="39672-145">displayName</span><span class="sxs-lookup"><span data-stu-id="39672-145">displayName</span></span>|<span data-ttu-id="39672-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39672-146">String</span></span>|<span data-ttu-id="39672-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="39672-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="39672-148">descrição</span><span class="sxs-lookup"><span data-stu-id="39672-148">description</span></span>|<span data-ttu-id="39672-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39672-149">String</span></span>|<span data-ttu-id="39672-150">O administrador forneceu a descrição do CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="39672-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="39672-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="39672-151">deviceCartIds</span></span>|<span data-ttu-id="39672-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="39672-152">String collection</span></span>|<span data-ttu-id="39672-153">Identificadores de carrinhos de dispositivo a serem associados a classes.</span><span class="sxs-lookup"><span data-stu-id="39672-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="39672-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="39672-154">classroomIds</span></span>|<span data-ttu-id="39672-155">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="39672-155">String collection</span></span>|<span data-ttu-id="39672-156">Identificadores de salas de aula a serem associadas a carrinhos de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="39672-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="39672-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="39672-157">Response</span></span>
<span data-ttu-id="39672-158">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39672-158">If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39672-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39672-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="39672-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39672-160">Request</span></span>
<span data-ttu-id="39672-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39672-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="39672-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="39672-162">Response</span></span>
<span data-ttu-id="39672-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39672-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "9bdc58dd-58dd-9bdc-dd58-dc9bdd58dc9b",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```




