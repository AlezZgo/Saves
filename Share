<SHARE>

private fun share() {
        viewModel.address.value?.data?.shortSlug?.let {
            val link = getString(R.string.deeplink_address, it)

            val sendIntent: Intent = Intent().apply {
                action = Intent.ACTION_SEND
                putExtra(Intent.EXTRA_TEXT, link)
                type = "text/plain"
            }

            val shareIntent = Intent.createChooser(sendIntent, null)
            startActivity(shareIntent)
        }
    }
