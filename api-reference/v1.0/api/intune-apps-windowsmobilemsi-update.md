---
title: Atualizar windowsMobileMSI
description: Atualiza as propriedades de um objeto windowsMobileMSI.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c09cf2208f77eecdf92e162335238e532f267bfc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551747"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="e6f99-103">Atualizar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="e6f99-103">Update windowsMobileMSI</span></span>

> <span data-ttu-id="e6f99-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6f99-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6f99-105">Atualiza as propriedades de um objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="e6f99-105">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6f99-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e6f99-106">Prerequisites</span></span>
<span data-ttu-id="e6f99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6f99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6f99-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6f99-109">Permission type</span></span>|<span data-ttu-id="e6f99-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e6f99-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6f99-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6f99-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e6f99-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6f99-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e6f99-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6f99-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6f99-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6f99-114">Not supported.</span></span>|
|<span data-ttu-id="e6f99-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6f99-115">Application</span></span>|<span data-ttu-id="e6f99-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6f99-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6f99-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6f99-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="e6f99-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6f99-118">Request headers</span></span>
|<span data-ttu-id="e6f99-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6f99-119">Header</span></span>|<span data-ttu-id="e6f99-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e6f99-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6f99-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6f99-121">Authorization</span></span>|<span data-ttu-id="e6f99-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6f99-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6f99-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e6f99-123">Accept</span></span>|<span data-ttu-id="e6f99-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e6f99-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6f99-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6f99-125">Request body</span></span>
<span data-ttu-id="e6f99-126">No corpo da solicitação, forneça uma representação JSON para o objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="e6f99-126">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="e6f99-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="e6f99-127">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="e6f99-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6f99-128">Property</span></span>|<span data-ttu-id="e6f99-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6f99-129">Type</span></span>|<span data-ttu-id="e6f99-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6f99-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6f99-131">id</span><span class="sxs-lookup"><span data-stu-id="e6f99-131">id</span></span>|<span data-ttu-id="e6f99-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6f99-132">String</span></span>|<span data-ttu-id="e6f99-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e6f99-133">Key of the entity.</span></span> <span data-ttu-id="e6f99-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6f99-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6f99-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e6f99-135">displayName</span></span>|<span data-ttu-id="e6f99-136">String</span><span class="sxs-lookup"><span data-stu-id="e6f99-136">String</span></span>|<span data-ttu-id="e6f99-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e6f99-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e6f99-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6f99-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6f99-139">description</span><span class="sxs-lookup"><span data-stu-id="e6f99-139">description</span></span>|<span data-ttu-id="e6f99-140">String</span><span class="sxs-lookup"><span data-stu-id="e6f99-140">String</span></span>|<span data-ttu-id="e6f99-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6f99-141">The description of the app.</span></span> <span data-ttu-id="e6f99-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6f99-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6f99-143">publicador</span><span class="sxs-lookup"><span data-stu-id="e6f99-143">publisher</span></span>|<span data-ttu-id="e6f99-144">String</span><span class="sxs-lookup"><span data-stu-id="e6f99-144">String</span></span>|<span data-ttu-id="e6f99-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6f99-145">The publisher of the app.</span></span> <span data-ttu-id="e6f99-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6f99-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6f99-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e6f99-147">largeIcon</span></span>|[<span data-ttu-id="e6f99-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e6f99-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e6f99-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e6f99-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e6f99-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6f99-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6f99-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6f99-151">createdDateTime</span></span>|<span data-ttu-id="e6f99-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6f99-152">DateTimeOffset</span></span>|<span data-ttu-id="e6f99-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6f99-153">The date and time the app was created.</span></span> <span data-ttu-id="e6f99-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6f99-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6f99-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6f99-155">lastModifiedDateTime</span></span>|<span data-ttu-id="e6f99-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6f99-156">DateTimeOffset</span></span>|<span data-ttu-id="e6f99-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e6f99-157">The date and time the app was last modified.</span></span> <span data-ttu-id="e6f99-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6f99-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6f99-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e6f99-159">isFeatured</span></span>|<span data-ttu-id="e6f99-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="e6f99-160">Boolean</span></span>|<span data-ttu-id="e6f99-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6f99-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6f99-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e6f99-162">privacyInformationUrl</span></span>|<span data-ttu-id="e6f99-163">String</span><span class="sxs-lookup"><span data-stu-id="e6f99-163">String</span></span>|<span data-ttu-id="e6f99-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e6f99-164">The privacy statement Url.</span></span> <span data-ttu-id="e6f99-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6f99-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6f99-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e6f99-166">informationUrl</span></span>|<span data-ttu-id="e6f99-167">String</span><span class="sxs-lookup"><span data-stu-id="e6f99-167">String</span></span>|<span data-ttu-id="e6f99-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e6f99-168">The more information Url.</span></span> <span data-ttu-id="e6f99-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6f99-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6f99-170">owner</span><span class="sxs-lookup"><span data-stu-id="e6f99-170">owner</span></span>|<span data-ttu-id="e6f99-171">String</span><span class="sxs-lookup"><span data-stu-id="e6f99-171">String</span></span>|<span data-ttu-id="e6f99-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e6f99-172">The owner of the app.</span></span> <span data-ttu-id="e6f99-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6f99-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6f99-174">developer</span><span class="sxs-lookup"><span data-stu-id="e6f99-174">developer</span></span>|<span data-ttu-id="e6f99-175">String</span><span class="sxs-lookup"><span data-stu-id="e6f99-175">String</span></span>|<span data-ttu-id="e6f99-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6f99-176">The developer of the app.</span></span> <span data-ttu-id="e6f99-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6f99-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6f99-178">notes</span><span class="sxs-lookup"><span data-stu-id="e6f99-178">notes</span></span>|<span data-ttu-id="e6f99-179">String</span><span class="sxs-lookup"><span data-stu-id="e6f99-179">String</span></span>|<span data-ttu-id="e6f99-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6f99-180">Notes for the app.</span></span> <span data-ttu-id="e6f99-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6f99-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e6f99-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="e6f99-182">publishingState</span></span>|[<span data-ttu-id="e6f99-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e6f99-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e6f99-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6f99-184">The publishing state for the app.</span></span> <span data-ttu-id="e6f99-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e6f99-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e6f99-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e6f99-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e6f99-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e6f99-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e6f99-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e6f99-188">committedContentVersion</span></span>|<span data-ttu-id="e6f99-189">String</span><span class="sxs-lookup"><span data-stu-id="e6f99-189">String</span></span>|<span data-ttu-id="e6f99-190">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="e6f99-190">The internal committed content version.</span></span> <span data-ttu-id="e6f99-191">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6f99-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e6f99-192">fileName</span><span class="sxs-lookup"><span data-stu-id="e6f99-192">fileName</span></span>|<span data-ttu-id="e6f99-193">String</span><span class="sxs-lookup"><span data-stu-id="e6f99-193">String</span></span>|<span data-ttu-id="e6f99-194">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="e6f99-194">The name of the main Lob application file.</span></span> <span data-ttu-id="e6f99-195">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6f99-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e6f99-196">size</span><span class="sxs-lookup"><span data-stu-id="e6f99-196">size</span></span>|<span data-ttu-id="e6f99-197">Int64</span><span class="sxs-lookup"><span data-stu-id="e6f99-197">Int64</span></span>|<span data-ttu-id="e6f99-198">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="e6f99-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="e6f99-199">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6f99-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e6f99-200">commandLine</span><span class="sxs-lookup"><span data-stu-id="e6f99-200">commandLine</span></span>|<span data-ttu-id="e6f99-201">String</span><span class="sxs-lookup"><span data-stu-id="e6f99-201">String</span></span>|<span data-ttu-id="e6f99-202">A linha de comando.</span><span class="sxs-lookup"><span data-stu-id="e6f99-202">The command line.</span></span>|
|<span data-ttu-id="e6f99-203">productCode</span><span class="sxs-lookup"><span data-stu-id="e6f99-203">productCode</span></span>|<span data-ttu-id="e6f99-204">String</span><span class="sxs-lookup"><span data-stu-id="e6f99-204">String</span></span>|<span data-ttu-id="e6f99-205">O código do produto.</span><span class="sxs-lookup"><span data-stu-id="e6f99-205">The product code.</span></span>|
|<span data-ttu-id="e6f99-206">productVersion</span><span class="sxs-lookup"><span data-stu-id="e6f99-206">productVersion</span></span>|<span data-ttu-id="e6f99-207">String</span><span class="sxs-lookup"><span data-stu-id="e6f99-207">String</span></span>|<span data-ttu-id="e6f99-208">A versão de produto do aplicativo de linha de negócios (LoB) Windows Mobile MSI.</span><span class="sxs-lookup"><span data-stu-id="e6f99-208">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e6f99-209">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="e6f99-209">ignoreVersionDetection</span></span>|<span data-ttu-id="e6f99-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6f99-210">Boolean</span></span>|<span data-ttu-id="e6f99-211">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e6f99-211">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="e6f99-212">Defina como true para o aplicativos de linha de negócios (LoB) Windows Mobile MSI que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="e6f99-212">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="e6f99-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6f99-213">Response</span></span>
<span data-ttu-id="e6f99-214">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6f99-214">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6f99-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6f99-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6f99-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6f99-216">Request</span></span>
<span data-ttu-id="e6f99-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6f99-217">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 855

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="e6f99-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6f99-218">Response</span></span>
<span data-ttu-id="e6f99-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6f99-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1027

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```



