# <a name="privacyprofile-resource-type"></a><span data-ttu-id="6d0df-101">Tipo de recurso privacyProfile</span><span class="sxs-lookup"><span data-stu-id="6d0df-101">privacyProfile resource type</span></span>

<span data-ttu-id="6d0df-102">Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="6d0df-102">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="6d0df-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d0df-103">Properties</span></span>
| <span data-ttu-id="6d0df-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d0df-104">Property</span></span>   | <span data-ttu-id="6d0df-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d0df-105">Type</span></span>|<span data-ttu-id="6d0df-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d0df-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d0df-107">contactEmail</span><span class="sxs-lookup"><span data-stu-id="6d0df-107">contactEmail</span></span>|<span data-ttu-id="6d0df-108">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d0df-108">String</span></span>| <span data-ttu-id="6d0df-109">Um endereço de email smtp válido para o contato da política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="6d0df-109">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="6d0df-110">Não obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d0df-110">not required</span></span>|
|<span data-ttu-id="6d0df-111">statementUrl</span><span class="sxs-lookup"><span data-stu-id="6d0df-111">statementUrl</span></span>|<span data-ttu-id="6d0df-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d0df-112">String</span></span>| <span data-ttu-id="6d0df-113">Um formato de URL válido começando por http:// ou https://.</span><span class="sxs-lookup"><span data-stu-id="6d0df-113">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="6d0df-114">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="6d0df-114">The maximum length is 255 characters.</span></span> <span data-ttu-id="6d0df-115">A URL que direciona para a política de privacidade da empresa.</span><span class="sxs-lookup"><span data-stu-id="6d0df-115">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="6d0df-116">Não obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d0df-116">not required</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d0df-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d0df-117">JSON representation</span></span>

<span data-ttu-id="6d0df-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6d0df-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```