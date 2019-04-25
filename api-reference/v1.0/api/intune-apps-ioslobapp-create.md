---
title: Criar iosLobApp
description: Cria um novo objeto iosLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b26dfa8330a2c00f8d51659a45000e3a04a5c66
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577459"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="5ebeb-103">Criar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="5ebeb-103">Create iosLobApp</span></span>

> <span data-ttu-id="5ebeb-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ebeb-105">Cria um novo objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5ebeb-105">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ebeb-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ebeb-106">Prerequisites</span></span>
<span data-ttu-id="5ebeb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ebeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ebeb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ebeb-109">Permission type</span></span>|<span data-ttu-id="5ebeb-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ebeb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5ebeb-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ebeb-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5ebeb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ebeb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-114">Not supported.</span></span>|
|<span data-ttu-id="5ebeb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ebeb-115">Application</span></span>|<span data-ttu-id="5ebeb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ebeb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ebeb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5ebeb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebeb-118">Request headers</span></span>
|<span data-ttu-id="5ebeb-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ebeb-119">Header</span></span>|<span data-ttu-id="5ebeb-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5ebeb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ebeb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ebeb-121">Authorization</span></span>|<span data-ttu-id="5ebeb-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ebeb-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ebeb-123">Accept</span></span>|<span data-ttu-id="5ebeb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5ebeb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ebeb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebeb-125">Request body</span></span>
<span data-ttu-id="5ebeb-126">No corpo da solicitação, forneça uma representação JSON do objeto iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-126">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="5ebeb-127">A tabela a seguir mostra as propriedades obrigatórias ao criar iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-127">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="5ebeb-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ebeb-128">Property</span></span>|<span data-ttu-id="5ebeb-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ebeb-129">Type</span></span>|<span data-ttu-id="5ebeb-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ebeb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ebeb-131">id</span><span class="sxs-lookup"><span data-stu-id="5ebeb-131">id</span></span>|<span data-ttu-id="5ebeb-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ebeb-132">String</span></span>|<span data-ttu-id="5ebeb-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-133">Key of the entity.</span></span> <span data-ttu-id="5ebeb-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ebeb-135">displayName</span><span class="sxs-lookup"><span data-stu-id="5ebeb-135">displayName</span></span>|<span data-ttu-id="5ebeb-136">String</span><span class="sxs-lookup"><span data-stu-id="5ebeb-136">String</span></span>|<span data-ttu-id="5ebeb-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5ebeb-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ebeb-139">description</span><span class="sxs-lookup"><span data-stu-id="5ebeb-139">description</span></span>|<span data-ttu-id="5ebeb-140">String</span><span class="sxs-lookup"><span data-stu-id="5ebeb-140">String</span></span>|<span data-ttu-id="5ebeb-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-141">The description of the app.</span></span> <span data-ttu-id="5ebeb-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ebeb-143">publicador</span><span class="sxs-lookup"><span data-stu-id="5ebeb-143">publisher</span></span>|<span data-ttu-id="5ebeb-144">String</span><span class="sxs-lookup"><span data-stu-id="5ebeb-144">String</span></span>|<span data-ttu-id="5ebeb-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-145">The publisher of the app.</span></span> <span data-ttu-id="5ebeb-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ebeb-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5ebeb-147">largeIcon</span></span>|[<span data-ttu-id="5ebeb-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5ebeb-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5ebeb-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5ebeb-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ebeb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ebeb-151">createdDateTime</span></span>|<span data-ttu-id="5ebeb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ebeb-152">DateTimeOffset</span></span>|<span data-ttu-id="5ebeb-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-153">The date and time the app was created.</span></span> <span data-ttu-id="5ebeb-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ebeb-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ebeb-155">lastModifiedDateTime</span></span>|<span data-ttu-id="5ebeb-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ebeb-156">DateTimeOffset</span></span>|<span data-ttu-id="5ebeb-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-157">The date and time the app was last modified.</span></span> <span data-ttu-id="5ebeb-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ebeb-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5ebeb-159">isFeatured</span></span>|<span data-ttu-id="5ebeb-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ebeb-160">Boolean</span></span>|<span data-ttu-id="5ebeb-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ebeb-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5ebeb-162">privacyInformationUrl</span></span>|<span data-ttu-id="5ebeb-163">String</span><span class="sxs-lookup"><span data-stu-id="5ebeb-163">String</span></span>|<span data-ttu-id="5ebeb-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-164">The privacy statement Url.</span></span> <span data-ttu-id="5ebeb-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ebeb-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5ebeb-166">informationUrl</span></span>|<span data-ttu-id="5ebeb-167">String</span><span class="sxs-lookup"><span data-stu-id="5ebeb-167">String</span></span>|<span data-ttu-id="5ebeb-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-168">The more information Url.</span></span> <span data-ttu-id="5ebeb-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ebeb-170">owner</span><span class="sxs-lookup"><span data-stu-id="5ebeb-170">owner</span></span>|<span data-ttu-id="5ebeb-171">String</span><span class="sxs-lookup"><span data-stu-id="5ebeb-171">String</span></span>|<span data-ttu-id="5ebeb-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-172">The owner of the app.</span></span> <span data-ttu-id="5ebeb-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ebeb-174">developer</span><span class="sxs-lookup"><span data-stu-id="5ebeb-174">developer</span></span>|<span data-ttu-id="5ebeb-175">String</span><span class="sxs-lookup"><span data-stu-id="5ebeb-175">String</span></span>|<span data-ttu-id="5ebeb-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-176">The developer of the app.</span></span> <span data-ttu-id="5ebeb-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ebeb-178">notes</span><span class="sxs-lookup"><span data-stu-id="5ebeb-178">notes</span></span>|<span data-ttu-id="5ebeb-179">String</span><span class="sxs-lookup"><span data-stu-id="5ebeb-179">String</span></span>|<span data-ttu-id="5ebeb-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-180">Notes for the app.</span></span> <span data-ttu-id="5ebeb-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5ebeb-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="5ebeb-182">publishingState</span></span>|[<span data-ttu-id="5ebeb-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5ebeb-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5ebeb-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-184">The publishing state for the app.</span></span> <span data-ttu-id="5ebeb-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5ebeb-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5ebeb-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5ebeb-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5ebeb-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="5ebeb-188">committedContentVersion</span></span>|<span data-ttu-id="5ebeb-189">String</span><span class="sxs-lookup"><span data-stu-id="5ebeb-189">String</span></span>|<span data-ttu-id="5ebeb-190">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-190">The internal committed content version.</span></span> <span data-ttu-id="5ebeb-191">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5ebeb-192">fileName</span><span class="sxs-lookup"><span data-stu-id="5ebeb-192">fileName</span></span>|<span data-ttu-id="5ebeb-193">String</span><span class="sxs-lookup"><span data-stu-id="5ebeb-193">String</span></span>|<span data-ttu-id="5ebeb-194">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-194">The name of the main Lob application file.</span></span> <span data-ttu-id="5ebeb-195">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5ebeb-196">size</span><span class="sxs-lookup"><span data-stu-id="5ebeb-196">size</span></span>|<span data-ttu-id="5ebeb-197">Int64</span><span class="sxs-lookup"><span data-stu-id="5ebeb-197">Int64</span></span>|<span data-ttu-id="5ebeb-198">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="5ebeb-199">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ebeb-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5ebeb-200">bundleId</span><span class="sxs-lookup"><span data-stu-id="5ebeb-200">bundleId</span></span>|<span data-ttu-id="5ebeb-201">String</span><span class="sxs-lookup"><span data-stu-id="5ebeb-201">String</span></span>|<span data-ttu-id="5ebeb-202">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-202">The Identity Name.</span></span>|
|<span data-ttu-id="5ebeb-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="5ebeb-203">applicableDeviceType</span></span>|[<span data-ttu-id="5ebeb-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="5ebeb-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="5ebeb-205">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="5ebeb-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5ebeb-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5ebeb-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5ebeb-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="5ebeb-208">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-208">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="5ebeb-209">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5ebeb-209">expirationDateTime</span></span>|<span data-ttu-id="5ebeb-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ebeb-210">DateTimeOffset</span></span>|<span data-ttu-id="5ebeb-211">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-211">The expiration time.</span></span>|
|<span data-ttu-id="5ebeb-212">versionNumber</span><span class="sxs-lookup"><span data-stu-id="5ebeb-212">versionNumber</span></span>|<span data-ttu-id="5ebeb-213">String</span><span class="sxs-lookup"><span data-stu-id="5ebeb-213">String</span></span>|<span data-ttu-id="5ebeb-214">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-214">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="5ebeb-215">buildNumber</span><span class="sxs-lookup"><span data-stu-id="5ebeb-215">buildNumber</span></span>|<span data-ttu-id="5ebeb-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ebeb-216">String</span></span>|<span data-ttu-id="5ebeb-217">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-217">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="5ebeb-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ebeb-218">Response</span></span>
<span data-ttu-id="5ebeb-219">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-219">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ebeb-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ebeb-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ebeb-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebeb-221">Request</span></span>
<span data-ttu-id="5ebeb-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1209

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="5ebeb-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ebeb-223">Response</span></span>
<span data-ttu-id="5ebeb-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ebeb-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1381

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



