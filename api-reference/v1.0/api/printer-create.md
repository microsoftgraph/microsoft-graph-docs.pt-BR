---
title: 'printer: create'
description: Crie (registre) uma impressora com o serviço Impressão Universal.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: bd07e04aa2a4c8b459e90a55d537c683a677d8e9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772041"
---
# <a name="printer-create"></a><span data-ttu-id="ce5d7-103">printer: create</span><span class="sxs-lookup"><span data-stu-id="ce5d7-103">printer: create</span></span>
<span data-ttu-id="ce5d7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce5d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="ce5d7-105">Crie (registre) uma impressora com o serviço Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-105">Create (register) a printer with the Universal Print service.</span></span> <span data-ttu-id="ce5d7-106">Esta é uma operação de longa duração e, como tal, retorna uma [printerCreateOperation](../resources/printercreateoperation.md) que pode ser usada para rastrear e verificar o registro da impressora.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-106">This is a long-running operation and as such, it returns a [printerCreateOperation](../resources/printercreateoperation.md) that can be used to track and verify the registration of the printer.</span></span>

<span data-ttu-id="ce5d7-107">Para ajudar a criar a CSR (Solicitação de Assinatura de Certificado) necessária para a criação da impressora, consulte o exemplo de código de geração [CSR](/universal-print/hardware/universal-print-oem-certificate-signing-request).</span><span class="sxs-lookup"><span data-stu-id="ce5d7-107">For help creating the required Certificate Signing Request (CSR) for creating printer, see the [CSR generation code sample](/universal-print/hardware/universal-print-oem-certificate-signing-request).</span></span>

## <a name="permissions"></a><span data-ttu-id="ce5d7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce5d7-108">Permissions</span></span>
<span data-ttu-id="ce5d7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce5d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ce5d7-111">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="ce5d7-112">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="ce5d7-112">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="ce5d7-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce5d7-113">Permission type</span></span> | <span data-ttu-id="ce5d7-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce5d7-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ce5d7-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce5d7-115">Delegated (work or school account)</span></span>| <span data-ttu-id="ce5d7-116">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="ce5d7-116">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="ce5d7-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce5d7-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce5d7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-118">Not Supported.</span></span>|
|<span data-ttu-id="ce5d7-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce5d7-119">Application</span></span>| <span data-ttu-id="ce5d7-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce5d7-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce5d7-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/create
```

## <a name="request-headers"></a><span data-ttu-id="ce5d7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce5d7-122">Request headers</span></span>
|<span data-ttu-id="ce5d7-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ce5d7-123">Name</span></span>|<span data-ttu-id="ce5d7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce5d7-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ce5d7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce5d7-125">Authorization</span></span>|<span data-ttu-id="ce5d7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ce5d7-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce5d7-128">Content-Type</span></span>|<span data-ttu-id="ce5d7-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce5d7-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce5d7-131">Request body</span></span>
<span data-ttu-id="ce5d7-132">No corpo da solicitação, fornece uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-132">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="ce5d7-133">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-133">The following table shows the parameters that can be used with this action.</span></span>

| <span data-ttu-id="ce5d7-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ce5d7-134">Parameter</span></span>      | <span data-ttu-id="ce5d7-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce5d7-135">Type</span></span>    |<span data-ttu-id="ce5d7-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce5d7-136">Description</span></span>| <span data-ttu-id="ce5d7-137">Obrigatório?</span><span class="sxs-lookup"><span data-stu-id="ce5d7-137">Required?</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="ce5d7-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ce5d7-138">displayName</span></span>|<span data-ttu-id="ce5d7-139">String</span><span class="sxs-lookup"><span data-stu-id="ce5d7-139">String</span></span>|<span data-ttu-id="ce5d7-140">O nome de exibição a ser atribuído à impressora.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-140">The display name to assign to the printer.</span></span>|<span data-ttu-id="ce5d7-141">Sim</span><span class="sxs-lookup"><span data-stu-id="ce5d7-141">Yes</span></span>|
|<span data-ttu-id="ce5d7-142">fabricante</span><span class="sxs-lookup"><span data-stu-id="ce5d7-142">manufacturer</span></span>|<span data-ttu-id="ce5d7-143">String</span><span class="sxs-lookup"><span data-stu-id="ce5d7-143">String</span></span>|<span data-ttu-id="ce5d7-144">O fabricante da impressora.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-144">The manufacturer of the printer.</span></span>|<span data-ttu-id="ce5d7-145">Sim</span><span class="sxs-lookup"><span data-stu-id="ce5d7-145">Yes</span></span>|
|<span data-ttu-id="ce5d7-146">modelo</span><span class="sxs-lookup"><span data-stu-id="ce5d7-146">model</span></span>|<span data-ttu-id="ce5d7-147">String</span><span class="sxs-lookup"><span data-stu-id="ce5d7-147">String</span></span>|<span data-ttu-id="ce5d7-148">O modelo da impressora.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-148">The model of the printer.</span></span>|<span data-ttu-id="ce5d7-149">Sim</span><span class="sxs-lookup"><span data-stu-id="ce5d7-149">Yes</span></span>|
|<span data-ttu-id="ce5d7-150">physicalDeviceId</span><span class="sxs-lookup"><span data-stu-id="ce5d7-150">physicalDeviceId</span></span>|<span data-ttu-id="ce5d7-151">String</span><span class="sxs-lookup"><span data-stu-id="ce5d7-151">String</span></span>|<span data-ttu-id="ce5d7-152">O UUID do dispositivo físico da impressora.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-152">The physical device UUID of the printer.</span></span> <span data-ttu-id="ce5d7-153">Obrigatório se a `hasPhysicalDevice` propriedade for true.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-153">Required if the `hasPhysicalDevice` property is true.</span></span>|<span data-ttu-id="ce5d7-154">Não</span><span class="sxs-lookup"><span data-stu-id="ce5d7-154">No</span></span>|
|<span data-ttu-id="ce5d7-155">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="ce5d7-155">hasPhysicalDevice</span></span>|<span data-ttu-id="ce5d7-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce5d7-156">Boolean</span></span>|<span data-ttu-id="ce5d7-157">True se a impressora tiver um dispositivo de saída físico, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-157">True if the printer has physical output device, false otherwise.</span></span> <span data-ttu-id="ce5d7-158">Se omitido, o valor padrão será true.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-158">If omitted, the default value is true.</span></span>|<span data-ttu-id="ce5d7-159">Não</span><span class="sxs-lookup"><span data-stu-id="ce5d7-159">No</span></span>|
|<span data-ttu-id="ce5d7-160">certificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="ce5d7-160">certificateSigningRequest</span></span>|[<span data-ttu-id="ce5d7-161">printCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="ce5d7-161">printCertificateSigningRequest</span></span>](../resources/printcertificatesigningrequest.md)|<span data-ttu-id="ce5d7-162">A Solicitação de Assinatura de Certificado X.509 (CSR) para o certificado criado e usado pela impressora para se identificar.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-162">The X.509 Certificate Signing Request (CSR) for the certificate created and used by the printer to identify itself.</span></span>|<span data-ttu-id="ce5d7-163">Sim</span><span class="sxs-lookup"><span data-stu-id="ce5d7-163">Yes</span></span>|
|<span data-ttu-id="ce5d7-164">connectorId</span><span class="sxs-lookup"><span data-stu-id="ce5d7-164">connectorId</span></span>|<span data-ttu-id="ce5d7-165">String</span><span class="sxs-lookup"><span data-stu-id="ce5d7-165">String</span></span>|<span data-ttu-id="ce5d7-166">ID do conector atuando como proxy para a impressora.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-166">ID of the connector acting as proxy to the printer.</span></span>|<span data-ttu-id="ce5d7-167">Não</span><span class="sxs-lookup"><span data-stu-id="ce5d7-167">No</span></span>|

## <a name="response"></a><span data-ttu-id="ce5d7-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce5d7-168">Response</span></span>
<span data-ttu-id="ce5d7-169">Se tiver êxito, este método retornará um código de resposta e um link para `202 Accepted` a [impressora associadaCreateOperation](../resources/printercreateoperation.md) no `Operation-Location` header.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-169">If successful, this method returns a `202 Accepted` response code and a link to the associated [printerCreateOperation](../resources/printercreateoperation.md) in the `Operation-Location` header.</span></span>

<span data-ttu-id="ce5d7-170">Você faz uma solicitação GET para a URL vinculada para obter o status de um registro de impressora em andamento.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-170">You make a GET request to the linked URL to get the status of an ongoing printer registration.</span></span> <span data-ttu-id="ce5d7-171">Depois que o registro da impressora for concluído com êxito, uma solicitação GET para a URL vinculada conterá o objeto de impressora criado e o certificado registrado.</span><span class="sxs-lookup"><span data-stu-id="ce5d7-171">After printer registration has completed successfully, a GET request to the linked URL will contain the created printer object and registered certificate.</span></span>

## <a name="examples"></a><span data-ttu-id="ce5d7-172">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ce5d7-172">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce5d7-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce5d7-173">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ce5d7-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce5d7-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer_create"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/create
Content-Type: application/json
Content-length: 287

{
  "displayName": "Test Printer",
  "manufacturer": "Test Printer Manufacturer",
  "model": "Test Printer Model",
  "physicalDeviceId": null,
  "hasPhysicalDevice": false,
  "certificateSigningRequest": { 
    "content": "{content}",
    "transportKey": "{sampleTransportKey}"
  },
  "connectorId": null
}
```
# <a name="c"></a>[<span data-ttu-id="ce5d7-175">C#</span><span class="sxs-lookup"><span data-stu-id="ce5d7-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-create-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce5d7-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce5d7-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-create-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce5d7-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce5d7-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-create-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce5d7-178">Java</span><span class="sxs-lookup"><span data-stu-id="ce5d7-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printer-create-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ce5d7-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce5d7-179">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
Operation-Location: https://graph.microsoft.com/v1.0/print/operations/f221760a-52e8-4c11-b8c5-5dfaef3a49db
Retry-After: 5
```

