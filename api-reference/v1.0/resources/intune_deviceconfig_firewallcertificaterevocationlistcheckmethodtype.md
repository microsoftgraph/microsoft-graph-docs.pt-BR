# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="b0049-101">tipo enumerado firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="b0049-101">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="b0049-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b0049-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0049-103">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="b0049-103">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="b0049-104">Membros</span><span class="sxs-lookup"><span data-stu-id="b0049-104">Members</span></span>
|<span data-ttu-id="b0049-105">Membro</span><span class="sxs-lookup"><span data-stu-id="b0049-105">Member</span></span>|<span data-ttu-id="b0049-106">Valor</span><span class="sxs-lookup"><span data-stu-id="b0049-106">Value</span></span>|<span data-ttu-id="b0049-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0049-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0049-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b0049-108">deviceDefault</span></span>|<span data-ttu-id="b0049-109">0</span><span class="sxs-lookup"><span data-stu-id="b0049-109">0%</span></span>|<span data-ttu-id="b0049-110">Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="b0049-110">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="b0049-111">nenhum</span><span class="sxs-lookup"><span data-stu-id="b0049-111">none</span></span>|<span data-ttu-id="b0049-112">1</span><span class="sxs-lookup"><span data-stu-id="b0049-112">-1</span></span>|<span data-ttu-id="b0049-113">Não verificar a lista de revogação de certificado</span><span class="sxs-lookup"><span data-stu-id="b0049-113">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="b0049-114">tentativa</span><span class="sxs-lookup"><span data-stu-id="b0049-114">attempt</span></span>|<span data-ttu-id="b0049-115">2</span><span class="sxs-lookup"><span data-stu-id="b0049-115">-2</span></span>|<span data-ttu-id="b0049-116">Tente a verificação CRL e permita um certificado somente se o certificado for confirmado pela verificação</span><span class="sxs-lookup"><span data-stu-id="b0049-116">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="b0049-117">precisar</span><span class="sxs-lookup"><span data-stu-id="b0049-117">Require</span></span>|<span data-ttu-id="b0049-118">3</span><span class="sxs-lookup"><span data-stu-id="b0049-118">-3</span></span>|<span data-ttu-id="b0049-119">Exigir uma verificação CRL bem-sucedida antes de permitir um certificado</span><span class="sxs-lookup"><span data-stu-id="b0049-119">Require a successful CRL check before allowing a certificate</span></span>|








